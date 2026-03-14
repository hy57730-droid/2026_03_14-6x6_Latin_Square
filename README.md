# verbose-engine
A Python tool that generates unique-solution 6×6 Latin Square puzzles with three difficulty levels and exports them as printable PDFs.
6×6 のラテン方格パズルを自動生成し、難易度3段階で一意解を保証して PDF 出力できる Python プログラムです。
日本語は下にあります。 

6×6 Latin Square Puzzle Generator
A Python program that generates unique-solution 6×6 Latin Square puzzles and exports them as printable PDFs. Difficulty levels: A (Easy), B (Normal), C (Hard).
________________________________________
🇺🇸 English README
✨ Features
  •Random generation of 6×6 Latin square solutions
  •Difficulty levels: A (Easy), B (Normal), C (Hard)
  •Ensures unique-solution puzzles
  •Outputs puzzle as a PDF file (zeros are shown as blank cells)
  •PDF is saved in the same folder as the script

📁 Output Example
  •puzzle6x6.pdf — A clean, printable 6×6 puzzle layout on A4 paper.

🔧 Requirements
  •Python 3.8+
  •ReportLab
  Install:
	pip install reportlab
▶️ How to Use
    1.Clone or download this repository.
    2.Run the script:
  python puzzle_generator.py
    3.Choose a difficulty level:
      A = Easy
      B = Normal
      C = Hard
    4.The file puzzle6x6.pdf will be generated in the same folder.

🎮 Difficulty Levels
	Level	Hints per Row	Random Removal	Description
	A (Easy)	3	0	Suitable for children; many hints.
	B (Normal)	2	2	Balanced difficulty for adults.
	C (Hard)	2	4	Requires logical reasoning.

📄 PDF Layout
  •A4 size
  •25mm square cells
  •Centered 6×6 grid
  •Numbers centered in each cell
  •Zeros are displayed as blank cells

🧩 How It Works
  1. Generate a complete Latin square
     Backtracking ensures no repeated numbers in rows or columns.
  2. Place hints based on difficulty
    •Minimum hints per row
    •Additional random removals for higher difficulty
  3. Check for unique solution
    Backtracking solver ensures exactly one solution.
  4. Export to PDF
    Uses ReportLab to draw a clean, printable puzzle.

📜 License
  This project is released under the MIT License, but commercial use is prohibited.
  You may use, modify, and distribute this software for personal or non-commercial purposes only.
________________________________________
🇯🇵 日本語 README
✨ 特徴
  •6×6 ラテン方格の完成盤をランダム生成
  •難易度 A / B / C に応じてヒント数を調整
  •一意解になるまで自動で再生成
  •PDF に問題を出力（0 は空欄として表示）
  •PDF はスクリプトと同じフォルダに保存

📁 出力例
  •puzzle6x6.pdf — 6×6 のパズルが 1 ページに印刷用レイアウトで出力されます。

🔧 必要環境
  •Python 3.8+
  •ReportLab（PDF 出力用）
  インストール：
     pip install reportlab

▶️ 使い方
  1.このリポジトリをクローンまたは ZIP ダウンロード。
  2.ターミナルでスクリプトを実行：
   python puzzle_generator.py
  3.難易度を選択：
    A = やさしい
    B = ふつう
    C = むずかしい
  4.同じフォルダに puzzle6x6.pdf が生成されます。

🎮 難易度の違い
	難易度	行ごとのヒント数	ランダム削除	特徴
	A（やさしい）	3	0	小学生でも解けるレベル。ヒント多め。
	B（ふつう）	2	2	大人が楽しめる標準難易度。
	C（むずかしい）	2	4	推理が必要な難問。

📄 PDF レイアウト
  •A4 サイズ
  •1 マス 25mm の正方形
  •中央に 6×6 の盤面を配置
  •数字は中央揃え
  •0 は空欄として表示

🧩 仕組み
  1. ラテン方格の完成盤を DFS で生成
    行・列に同じ数字が入らないようにバックトラッキングで構築。
  2. 難易度に応じてヒントを配置
    •行ごとに最低ヒント数を確保
    •追加でランダムに削除（難易度アップ）
  3. 一意解チェック
    バックトラッキングで全解探索し、解が 1 つだけになるまで再生成。
  4. PDF 出力
    ReportLab を使って印刷用の盤面を描画。

📜 ライセンス
  本プロジェクトは MIT License に基づいて公開されていますが、商用利用は禁止されています。
  個人利用・非商用利用の範囲で自由に改変・再配布できます。
