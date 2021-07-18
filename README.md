# jrace
Java implementation of racing based automatic algorithm configurators.

Example run: 
`java -cp bin:lib/slf4j-api-1.7.5.jar:lib/logback-classic-1.0.13.jar:lib/logback-core-1.0.13.jar tune.Tuner -s random/scenario.txt`

To compile from source: `javac -d bin -cp lib/slf4j-api-1.7.5.jar:lib/logback-classic-1.0.13.jar:lib/logback-core-1.0.13.jar $(find . -name *.java)`

## Usage
Follow the the steps below to configure your algorithm with jrace:
1. Create a directory to store configuration scenarios
```bash
mkdir tuning
cd tuning
```
2. Copy scenario template and parameter template file
```bash
cp ../params.tmpl params.txt
cp ../scenario.tmpl scenario.txt
```
3. Put the directory of training instances in `scenario.txt`
