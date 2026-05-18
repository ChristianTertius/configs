# espanso match file

# For a complete introduction, visit the official docs at: https://espanso.org/docs/

# You can use this file to define the base matches (aka snippets)
# that will be available in every application when using espanso.

# Matches are substitution rules: when you type the "trigger" string
# it gets replaced by the "replace" string.

# yaml-language-server: $schema=https://raw.githubusercontent.com/espanso/espanso/dev/schemas/match.schema.json

matches:
  # Simple text replacement
  - trigger: ":espanso"
    replace: "Hi there!"
  - trigger: "ccn"
    replace: "Christian Carlos Tertius"
  - trigger: "cce"
    replace: "christian160103@gmail.com"
  - trigger: ":nik"
    replace: "7171051601030001"
  - trigger: ":nim"
    replace: "2501987803"
  - trigger: "cca"
    replace: "Jl. Budi Raya No.21, RT.1/RW.5, Kb. Jeruk, Kec. Kb. Jeruk, Kota Jakarta Barat, Daerah Khusus Ibukota Jakarta 11530"
  - trigger: "ccp"
    replace: "PT Prodia Widyahusada Tbk"
  - trigger: "ccp"
    replace: "Fullstack Developer Intern"
  - trigger: "ccr"
    replace: "Kinanti"
  - trigger: "ccr"
    replace: "087889965161"
  - trigger: "ccp"
    replace: "● Developed and maintained three internal systems using PHP (Laravel & CodeIgniter), collaborating with IT
teams and optimizing MySQL databases for better performance.

● Independently developed a referral application and a data parsing tool from scratch, handling frontend,
backend, and database design, successfully deployed for internal use, improving workflow efficiency and
reducing manual workload.

● Assisted in debugging, testing, and implementing new features across systems, enhancing internal
operations and user experience.
"
  - trigger: "ccs"
    replace: "https://www.linkedin.com/in/christian-carlos-tertius/"
  - trigger: "ccs"
    replace: "https://instagram.com/christian_christer"
  - trigger: ":jurnal"
    replace: "Tanjung Priok Port is an international port in Indonesia located in Tanjung Priok, North Jakarta. For all activities carried out at Tanjung Priok Port to run smoothly, this research was made which aims to predict the height of tides using the Artificial Neural Network (ANN) and Decision Tree methods with a quantitative approach. Artificial Neural Network (ANN) is a technique inspired by the way the biological nervous system works, namely in brain cells in processing information received by humans. while Decision Tree is also known as a decision tree which is an algorithm for building a decision hierarchy structure. The process of making a Decision Tree starts from the Root Node to the Leaf Node which is done recursively. This research was conducted to predict the height of tides in January 2018 - June 2018. By using both methods that have been computed, the ANN method produces a smaller MSE value than the Decision Tree method. The ANN method produces an MSE value of 0.003727983. While the Decision Tree method produces an MSE value of 0.009870259. If the dataset used has larger amount of data and the architecture of each algorithm is more complex, then the calculation results obtained will be more accurate."
  - trigger: ":jurnal"
    replace: "Comparing Artificial Neural Network and Decision Tree Algorithm to Predict Tides at Tanjung Priok Port"

  # NOTE: espanso uses YAML to define matches, so pay attention to the indentation!

  # But matches can also be dynamic:

  # Print the current date
  - trigger: ":date"
    replace: "{{mydate}}"
    vars:
      - name: mydate
        type: date
        params:
          format: "%m/%d/%Y"

  # Print the output of a shell command
  - trigger: ":shell"
    replace: "{{output}}"
    vars:
      - name: output
        type: shell
        params:
          cmd: "echo 'Hello from your shell'"

  # And much more! For more information, visit the docs: https://espanso.org/docs/
