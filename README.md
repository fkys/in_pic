# in_pic
Python-CLI program to hide and extract data inside picture file  

## Instalation
```sh
git clone --depth=1 https://github.com/fkys/in_pic 
cd in_pic
chmod +x in_pic
```

## Usage
```sh
./in_pic -h # display help msg
./in_pic file-src file-dest # hide file-src in file-dest
./in_pic -o file_src [file-dest] # extract data from file-src
```

## How it works?
It append the data of the file that you want to hide to the end of jpg file and it stores the EOF coordinates of original jpg file in .eof.txt file, so when extracting the data it reads from the coordinate onward.  
initially i didn't use this technique but somehow it doesn't work with every jpg file so i did it this way

## References
- https://www.youtube.com/watch?v=r-7d3w5xerY
- https://upload.wikimedia.org/wikipedia/commons/thumb/3/38/Alpen_Edelwei%C3%9F%2C_Leontopodium_alpinum_2.JPG/1024px-Alpen_Edelwei%C3%9F%2C_Leontopodium_alpinum_2.JPG  

## 
> if you want funni try extracting img.jpeg
