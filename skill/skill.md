# vscode
> 在json文件中，一般默认为“${file}",所以只能进行当前文件的编译运行
> - 如果想明确编译那些文件，则将上面的东西替换为要编译的每个文件名：”main.cpp“，”add.cpp"
> - 如果想让vscode自动编译目录中所有的cpp文件，则替换为”${fileDirname}/**/*.cpp
> - 如果想让vscode自动编译当前目录下的非子目录的cpp文件，则替换为“${fileDirname}/*.cpp"
>
> 如果想在vscode中支持多路径搜索：
> - 在 tasks.json 配置文件中，在“Args”部分添加新行：
> - "-I/source/includes",