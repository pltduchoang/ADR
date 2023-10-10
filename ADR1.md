# **Architectural Decision Record (ADR)** 

Title: Selection of App Type (Native, Web, or Hybrid) for University
Social Networking App 

Context: We must decide on the type of application (native, web, or
hybrid) that will be developed for the university social networking app.
This decision will significantly impact the app's development, user
experience, and cross-platform compatibility. 

Decision: We have decided to develop a **hybrid app** for the university
social networking app. 

## **Rationale:** 

- **Cross-Platform Compatibility:** A hybrid app allows us to develop a
  > single codebase that can be deployed on both iOS and Android
  > platforms. This ensures widespread adoption and accessibility,
  > catering to students and professors using a variety of devices and
  > operating systems. 

- **Code Reusability:** Developing a hybrid app promotes code
  > reusability, as a significant portion of the codebase can be shared
  > between iOS and Android versions. This reduces development effort
  > and simplifies maintenance. 

- **Development Efficiency:** A hybrid app development approach is
  > generally more efficient than developing separate native apps for
  > iOS and Android. It allows the team to save time and resources by
  > maintaining a single codebase. 

- **Consistency:** Hybrid apps offer a consistent user interface and
  > user experience across both platforms, ensuring that users have a
  > cohesive and familiar interaction with the app. 

- 

## **Consequences:** 

- **Performance Issues**: Hybrid apps often suffer from slower
  > performance compared to fully native apps. This is because they rely
  > on a WebView to render the user interface, which can be less
  > efficient than native UI components. This can lead to issues like
  > slower load times and less smooth animations. 

- **UI/UX Consistency**: Achieving a consistent and polished user
  > interface across different platforms (iOS, Android, etc.) can be
  > challenging in hybrid development. Native apps can offer a more
  > platform-specific and seamless user experience. 

- **Limited Offline Functionality**: Hybrid apps may not work as well
  > offline as native apps. While some offline capabilities can be
  > implemented, they may not be as robust or reliable as what you can
  > achieve in a fully native app. 
