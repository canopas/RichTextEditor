# RichEditor

Android WYSIWYG Rich editor for Jetpack compose.

<img src="./gif/sample.gif" height="540" />

## Features

The editor offers the following <b>options</b>:

- [x] **Bold**
- [x] *Italic*
- [x] <u>Underline</u>
- [x] Different Heading

## How to add in your project

Add the dependency

```gradle
 implementation 'com.canopas.editor:rich-editor-compose:X.X.X'
```

## How to use ?

```
@Composable
fun Sample() {

        val context = LocalContext.current
        
        val state = remember {
            val input = /* YOUR INPUT */
            RichEditorState.Builder()
                .setInput(input)
                .adapter(JsonEditorParser())
                .build()
        }

        RichEditor(
                state = state,
                modifier = Modifier
                    .fillMaxWidth()
                    .weight(1f)
                    .border(1.dp, Color.Gray)
                    .padding(5.dp)
            )
    
}
```
# Demo
[Sample](https://github.com/canopas/RichEditorCompose/tree/main/app) app demonstrates how simple the usage of the library actually is.

# Bugs and Feedback
For bugs, questions and discussions please use the [Github Issues](https://github.com/canopas/RichEditorCompose/issues).


## Credits
RichEditor for compose is owned and maintained by the [Canopas team](https://canopas.com/). For project updates and releases, you can follow them on X at [@canopassoftware](https://x.com/canopassoftware).

ComposeRichEditor: https://github.com/MohamedRejeb/Compose-Rich-Editor

# Licence

```
Copyright 2023 Canopas Software LLP

Licensed under the Apache License, Version 2.0 (the "License");
You won't be using this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
