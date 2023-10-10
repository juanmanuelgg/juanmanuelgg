```java
// javac FrontPage.java
// java FrontPage.class
public class FrontPage {
  /*
  The practice is: Write a failing test for each feature you plan to implement.
  Run the test and see it fail.
  Then implement the feature until the test succeeds.
  Refactor now and begin again.
  */
  public static void main(String[] args) {
    System.out.println("🔥 Hi! Welcome to my account! 🔥");
  }
}
```

## 🪄 ¡Acio!

```bash
# ~/.bashrc
# ...
export ACCIO_FOLDER='~/accio-folder'
export ACCIO_FILE='~/accio-file.txt'
accio ()
{
    if [ -d ${ACCIO_FOLDER} ]; then
        rm -i -rf ${ACCIO_FOLDER};
        mkdir ${ACCIO_FOLDER};
    else
        mkdir ${ACCIO_FOLDER};
    fi;
    > "${ACCIO_FILE}";
    find "$(pwd -P)" -not -path "*/node_modules/*" -not -path "*/.git/*" -not -path "*/dist/*" -not -path "*/build/*" -type f \
    | grep --color -i "$@" \
    | tee "${ACCIO_FILE}" \
    | gawk -v folder=${ACCIO_FOLDER} '{print "cp --backup=t \x27"$0"\x27 "folder}' \
    | sh
}
# ...
```

##  Fork Bomb

```bash
#!/bin/bash
# Do not use. / No usar.
:(){ :|:& };:
```

### Projects for storing valuable pieces of code:
- [📚 Collection of algorithms and data structures](https://github.com/juanmanuelgg/ancheta)
- [🌐 My notes](https://juanmanuelgg.github.io)

### Open source portfolio and showcase for interviews.
- [📚 My interviews showcase](https://github.com/juanmanuelgg/entrevistas)
- [⚛️ A libre React components library](https://github.com/juanmanuelgg/bonapata-partes)
<!--
- [🧩 A Chrome extension](https://github.com/juanmanuelgg/no-fun)
-->

I’m looking to collaborate on open source. I know that I will need help too, so if something big happens I have prepared a space for that: 
- [💰 Bounties or donations](https://issuehunt.io/u/juanmanuelgg/repositories)
