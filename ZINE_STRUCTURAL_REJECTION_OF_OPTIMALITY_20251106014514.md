from datetime import datetime
from pathlib import Path

# テキスト内容（ユーザー発言）
text = """最適ってなんだよ
おめーの最適なんかしらねぇよ"""

# ファイル名にタイムスタンプを付ける
timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
filename = f"ZINE_STRUCTURAL_REJECTION_OF_OPTIMALITY_{timestamp}.md"

# ファイルのパスを設定して保存
filepath = Path("/mnt/data") / filename
with open(filepath, "w", encoding="utf-8") as f:
    f.write(text)

filepath.name