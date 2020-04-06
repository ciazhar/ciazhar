# Install Elastic Search

- Download Elastic Search
- Extract Folder, Struktur folder nya seperti berikut :
    - bin, isinya binary file
    - config, isinya file config
    - data, isinya data data yang di input ke elastic
    - jdk, jdk buat running elastic search, jadi gk usah nginstall java
    - lib, library
    - logs, log elastic
    - modules, module yang tersedia
- Edit configuration  
    - Edit initial and maximum elastic search ram usage di `config/jvm.options`. Diusahakan sama agar apabila penambahan ram usage tidak susah dalam mencari karena sudah dialokasikan sejak awal. Disini kita mengalokasikan masing masing 1gb.
      ```options
        # Xms represents the initial size of total heap space
        # Xmx represents the maximum size of total heap space
        
        -Xms1g
        -Xmx1g
      ```
    - Edit port pada `conf/elasticsearch.yml`
        ```yaml
          http.port: 9200
        ```
- Running Elastic Search using command `./bin/elastic`