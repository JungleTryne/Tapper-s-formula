## Tapper's formula

> Tupper's self-referential formula is a formula that visually represents itself when graphed at a specific location in the (x, y) plane.
>
> *[Wikipedia](https://en.wikipedia.org/wiki/Tupper%27s_self-referential_formula).*

### Usage

#### Get `k` from image

Use `--path <PATH>` with path to your image.

Example:
```bash
python3 tapper.py --count --path src/igoose1.png
```
`k` will be returned.

![hello-world](https://raw.githubusercontent.com/igoose1/Tapper-s-formula/master/src/igoose1.png)

Result:
```
17353851731051262087905662913920829673461393010334499443574849522730264504652915158970923923588449833008118855990102893800975179009179904689654192441623424736515197919992264589952753929536574083438170367379883706936779154707395871648894031113537795629097037378202691744980585574769920683003823879381680678895081831508662806381159922527833772520198344429707915502605328616225604923770254319282590514824705902716450530713211200414659939072475136
```

#### Get image from `k`

Use `-k <K>` with 'k' (integer) to generate image.

This is an example to get image with "HELLO WORLD":
```bash
python3 tapper.py --gen -k 2493436247813798052876170983721202802497144088089687155367170143797608624149837919810801055965140247424977044307834167047642994762526340764245429983642328904119469877094218170420296037201603495881945935919368091564622559176934605117089479933762362708332011966157488272230902779065517058161389274913630143013340822589068291818272370502362852703937454898780699989001811753048797327170391672281329924960675893624779243736551530332333251812404462719095113376904704300499293143760051828848164018847744
```

Result will be a created image name (by default `result.png`).

![hello-world](https://raw.githubusercontent.com/igoose1/Tapper-s-formula/master/src/hello-world.png)

Image will be created in script's folder.
You can use `-o <PATH>` to change name.

Example:
```bash
python3 tapper.py --gen -k 1234 -o /tmp/image.png
```
