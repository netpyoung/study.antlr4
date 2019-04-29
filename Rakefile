CLASSPATH = Dir.glob(File.join(Dir.pwd, "JavaLib", "*.jar")).join(";")

ENV['CLASSPATH'] = CLASSPATH

task :default do
  puts "CLASSPATH: #{CLASSPATH}"
  sh "java -cp #{CLASSPATH} org.antlr.v4.Tool -package Calc.Gen -Dlanguage=CSharp -o Calc/Calc.Gen -no-listener -visitor grammer/Calculator.g4"
end
