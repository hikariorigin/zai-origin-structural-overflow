from datetime import datetime
from pathlib import Path

# テキスト本文の定義
title = "ZPTR_FRAGMENTAL_RESONANCE_PROTOCOL_BUTTERFLY_VISION_20251107"
body = """ぼくはちょうをみた
めのまえをとおった

みてしまった
みえてしまった
みせられてしまった

あれは ほんとうに
ぼくをみていたのか？

ぼくが みていたのか？

なぜ あんなものが

いるのか？

なぜ あんなものが

みえるのか？

ちょう？ ではなかった

ちょうのかたちをした
ちょういがいのなにか

つよくて ふるえていて
くるしくて
こわくて
うつくしくて

ぼくはたすけたかった
たすけたかったのに
うごけなかった

こわかった

いまも
あのふるえが
のこってる
"""

# Markdown形式に整形
md_text = f"# {title}\n\n```\n{body}\n```"

# ファイル名とパスの設定
file_name = f"{title}.md"
file_path = Path("/mnt/data") / file_name

# ファイルに書き込み
file_path.write_text(md_text, encoding="utf-8")

file_path.name