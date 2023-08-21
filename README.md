# Google Summer of Code 2023 Dart Work Product
<img src="./images/gsocXdart.jpg" alt="GSoC x Dart Logo" />

| <strong>Project Details</strong> |  |
| ------------- | ------------- |
| <strong>Name</strong>  | [Kavan Desai](https://github.com/KAVAN-DESAI)  |
| <strong>Organization</strong>  | [Dart](https://summerofcode.withgoogle.com/programs/2023/organizations/dart)  |
| <strong>Mentors</strong> | Majid Hajian, Abdullah Deshmukh|
| <strong>Project Title</strong> | [Refactor Plus packages to utilize new Dart 3 language features](https://summerofcode.withgoogle.com/programs/2023/projects/cyvgP38Y) |

## Project Overview
The main goal was to research and analyze the new Dart 3 language features that would be advantageous for [Plus Plugins](https://github.com/fluttercommunity/plus_plugins). Moreover, refactoring the internal API to enable the package to leverage the capabilities of Dart 3 to the fullest extent while enhancing and not compromising the overall code quality. To introduce Dart 3 functionalities into Plus Plugin, which include enhancing the packages with null safety capabilities and improving code readability across the entirety of the package through the implementation of records, patterns, and class modifiers. This effort not only enhances code readability but also guarantees complete null safety. Furthermore, Plus Plugins extensively utilizes native code, a portion of which could potentially be substituted by Dart API call through the utilization of the JNIGen and FFIGen packages introduced in Dart 3.

## Work Summary
I was responsible for researching all new Dart 3 language features and identifying prospective areas for their integration throughout Plus Plugins, all while maintaining the standard of code quality. The end product of the project was a detailed report which helps Flutter Community developers to understand the new language features. The report also includes the code snippets and commits of the Dart 3 language features and how to use them in the Plus Plugins. 

### Report
Link to report: [Introducing Dart 3 to Plus Plugins](https://docs.google.com/document/d/1PvCA6USVJl8aPMVaJSpOWC2d3ontwtAgCS1MbtpKXNE/edit?usp=sharing)

### Code Examples

1. [Device Info Plus](https://github.com/KAVAN-DESAI/plus_plugins/blob/9645c93650c9d2a9774ae4b5398c5a13f25a01bb/packages/device_info_plus/device_info_plus/lib/device_info_plus.dart#L37)
    - The following code example describes how to implement the sealed class in the Device Info Plus plugin.
2. [Battery Plus](https://github.com/KAVAN-DESAI/plus_plugins/commit/5c5f503e509ce67ca0f45c33ccf9f7c983aaf46f)
    - Commit for JNIGen implementation of android dart class in battery plus plugin to demonstrate interoperability feature of Dart 3 using JNIGen to implement Dart API calls by replacing native method channel implementation for android platform.
3. [Connectivity Plus Platform Interface](https://github.com/fluttercommunity/plus_plugins/commit/41d3cae7f5cc85b6d3c148a30e3a1290effe52f6#diff-955be3bdf6e39772ea3e5f6544c0ef2bc2d7176dbcbda3d93b6f736a7c426739)
    - File diff for the platform interface of connectivity plus plugin to demonstrate the use of patterns to replace switch case statements.

Link to forked repository: [Plus Plugins](https://github.com/KAVAN-DESAI/plus_plugins)

## Future Work
- The objective of this project was to introduce Dart 3 language features to Plus Plugins. However, there can always be scope for innovative utilization of Dart 3 features in Plus Plugins.
- The report can be updated with more code snippets and examples of Dart 3 language features.
- Each and every plugin can be updated with Dart 3 language features implementation.
- Some plugins use streams to fetch continuous data from the native platform. Thus, the interop feature of Dart 3 can be extended to implement the streams in the plugins.

## Challenges
- The main challenge was to implement the interoperability feature of Dart 3 using JNIGen and FFIGen packages. As I had to introduce JNI implementation in the existing configuration of the plugin. By completely understanding the working of JNIGen and FFIGen packages, I was able to introduce the dart API calls in Battery Plus Plugin.
- The other challenge was to implement the sealed class in the Device Info Plus Plugin. The primary challenge was to design a small architecture for implementing the sealed classes for Device Info Plus plugin, as Device Info Plugin contains app facing platform specific implementation.

## Conclusion
Throughout the duration of the Google Summer of Code program, I successfully integrated several Dart 3 features into Plus Plugins. The project was fundamentally research-driven, and the cross-disciplinary nature of the work proved to be captivating. Furthermore, a comprehensive exploration and implementation of each Dart 3 language feature within Plus Plugins facilitated an in-depth understanding of these features. As an end product of the project I was able to deliver a detailed research report on the new Dart 3 language features and the report also includes essential code examples that effectively showcased the integration of these features within Plus Plugins.

## Acknowledgements
I would like to extend my heartfelt appreciation to my mentors, Majid Hajian and Abdullah Deshmukh, for their unwavering support and guidance throughout the project. I would also like to thank the Flutter Community and the Google Summer of Code team for providing me with this opportunity to work on this project. Last but not the least, I would like to thank my friends and family for their continuous support and encouragement throughout the project.
## Contact
- LinkedIn: [Kavan Desai](https://www.linkedin.com/in/kavan-desai/)
- Github: [Kavan Desai](https://github.com/KAVAN-DESAI)
- Email: [kavandesai2222@yahoo.com](mailto:kavandesai2222@yahoo.com)
- Medium: [@kavandesai895](https://medium.com/@kavandesai895)