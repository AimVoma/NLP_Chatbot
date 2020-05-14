
### Chatbot project

Project Assignment for Coursera 'Advanced Natural Language Processing' course offered by Moscow's
HSE University. The objective was to support a Chat-Bot application with Dual Intent Recognition, General QA and Programmatic Assistance. The General QA function was implemented by Chatterbot premade Python API. The Programmatic StackOverflow Assistance was based on word augmentation and text similarity extraction between the user questions and answers provided by StackOverflow cached history. 

### Project Structure
week5-project.ipynb -- (Text Preprocessing, Intent Classifier, Word Augmentation)<br/>
main_bot -- (Telegram Bot Handler Logic)<br/>
dialogue_manager -- (Thread Ranking , Chatbot's Dialogue Manager(requests-responses))<br/>
utils -- (Helping Functions) <br/>

### Tech
● AWS, Docker, Sklearn, Gensim, Word Embeddings, Chatterbot, Telegram API

### Preview
https://imgur.com/a/LQOxJ1F

### Future Improvements

The **poor General QA support** through **Chatterbot API** need to be remodeled at least in more dialogue coherent and natural state. Instead of generating patent/heuristic based static text generation. A good solution for Question - Answering dialogue modeling would be with Machine Translation(MT) with Attention modeling. Since in our user-bot dialogue we have independent sequence lengths, we can use Transformer Architecture to model the encoding (user sentence) and the decoding(bot-generated) answer. Perfect example of **Tensorflow Implementation** of MT tasks is a translation from one Language sequance to Another. By improvising the training data(Pair Dialogue), this can be used with this codebase [Neural machine translation with attention
Tensorflow[FR-EN]](https://www.tensorflow.org/tutorials/text/nmt_with_attention)


