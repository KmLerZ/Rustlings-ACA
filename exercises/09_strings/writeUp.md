# Résolution last exercice:

string_slice("blue"); -> string_slice attends une référence en argument (book exemple :fn first_word(s: &String) -> ?)

string("red".to_string()); -> .to_string est utilisé et n'attends pas de référence

string(String::from("hi")); -> String::from est utilisé et n'attends pas de référence

string("rust is fun!".to_owned()); -> .to_owned est utilisé et n'attends pas de référence

string("nice weather".into()); -> .into est utilisé et n'attends pas de référence

string(format!("Interpolation {}", "Station")); -> format! est utilisé et n'attends pas de référence

string_slice(&String::from("abc")[0..1]); -> Il fait une référence avec le "&"String

string_slice("  hello there ".trim()); -> .trim attends une référence (book exemple :pub fn trim(&self) -> &str)

string("Happy Monday!".to_string().replace("Mon", "Tues")); -> .to_strinf est utilisé et n'attends pas de référence

string("mY sHiFt KeY iS sTiCkY".to_lowercase()); -> .to_lowercase est utilisé et n'attends pas de référence
