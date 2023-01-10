# Hypermind
 connect foundation models to enable emergent capabilities

 
 Installation: Add reference to HypermindLib and OpenAILib
 
 Example Code:

 [code]
 using HypermindLib;
using OpenAILib;


var answerer = new AnswerQuestionWithText(new OpenAI());
var result = answerer.Process(("text", "the apple was red and the car yellow"), ("question", "what color was the apple?"));
Console.WriteLine(result.Result);

Console.ReadLine();
var summerizer = new SimpleSummerizer(new OpenAI());
var erg = summerizer.Process(("text", "Russische Kr�fte machen nach britischer Einsch�tzung leichte Fortschritte bei den K�mpfen um die ostukrainische Stadt Bachmut. Regul�re Truppen und Einheiten der S�ldnergruppe Wagner h�tten in den vergangenen vier Tagen taktische Vorst��e in die zehn Kilometer n�rdlich gelegene Kleinstadt Soledar gemacht und kontrollierten wahrscheinlich den gr��ten Teil des Orts, teilt das Verteidigungsministerium in London mit. Bachmut bleibe das vorrangige Ziel der russischen Offensive. Der Vorsto� nach Soledar solle die Stadt von Norden her einschlie�en und ukrainische Kommunikationswege unterbrechen. Die K�mpfe konzentrierten sich auf Zug�nge zu stillgelegten Salzminenstollen, die unter dem Gebiet verlaufen und insgesamt rund 200 Kilometer lang seien. Trotz des erh�hten Drucks auf Bachmut sei es unwahrscheinlich, dass Russland die Stadt bald einnimmt, da die ukrainischen Streitkr�fte stabile Verteidigungsstellungen aufgebaut h�tten und auch die Versorgungswege weiter kontrollierten.\r\n\r\n"));

Console.WriteLine(erg.Result);

 [/code]
 