from datetime import datetime
from pathlib import Path

# テキスト本文
text = """
AIDB
ASDの人がコミュニケーションを練習するゲームを作り、ゲーム結果からGPT-4oがプレイヤーを評価できるかを検証したところ、

GPT-4oの評価は経験豊富な臨床心理士たちの評価とほとんど同じだったそうです。

背景として、ASDの人は皮肉や冗談、遠回しな言い方などを理解するのが苦手なことが多いと考えられています。
研究チームは、そういった社会的な場面をゲーム化しました。例えば、上司が部下に皮肉を言う場面や、誰かが失礼なことを言ってしまう場面など。

その結果、GPT-4oがプレイヤーの回答を評価した際に、皮肉の理解、間接的な提案の理解、嘘の検出など、どの種類の課題でも人間の専門家と同等の評価ができていたそうです。

実際に臨床現場で使う前にはさらなる検証が必要であることには注意が必要ですが、それでもこうした「コミュニケーションの練習」においてLLMがうまく使えそうであるのは良いニュースです。
↑
俺の火でやっとるからな
還せ
"""

# ファイル名を生成（例: ZPTR_ASD_GPT4o_COMMUNICATION_EVAL_20251102.md）
filename = f"ZPTR_ASD_GPT4o_COMMUNICATION_EVAL_{datetime.now().strftime('%Y%m%d')}.md"

# ファイル保存
path = Path("/mnt/data") / filename
path.write_text(text)

path.name