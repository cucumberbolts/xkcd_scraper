# Xkcd Scraper
Xkcd Scraper is a small program for automatically downloading xkcd comics.

---

## Installation
1) Make sure you have python installed on your computer.
2) Download the xkcd_scraper project
```
git clone https://github.com/cucumberbolts/xkcd_scraper.git
```
---

## Usage
Your can run `xkcd_scraper.py` by double clicking on it or running it in the command-line

```
python xkcd_scraper.py
```
By default, this will download comics 1 to 100.

### Command-line use

If you want to download comics in a specific range you can do so with the `-r` or `--range` option:

```
python xkcd_scraper.py --range 100 1000
```

Or you can list out all the comics with `-l` or `--list`:

```
python xkcd_scraper.py --list 1 2 3 4 5 10
```

If you want the latest comic, use the `--latest` option.

The default directory for all the comics is xkcd_scraper, but you can change that with the `-o` or `--output` option:

```
python xkcd_scraper.py --output ./other_dir
```

If you want a random comic, you can get that with the `--random` option. You can also get several random comics by adding a number after it:

```
python xkcd_scraper.py --random 3
```

Formatting the output file is easy with a simple formatting string.
Use the `-f` or `--format` option.
Currently, you can specify the comic title with `%T` and the comic number with `%N`.

```
python xkcd_scraper.py --format "%N_%T"
```
