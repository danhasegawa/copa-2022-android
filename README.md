# App Android Copa 2022

In this project, we will create an application exploring the features of Android Jetpack.
The application will show the 2022 World Cup games and send you notifications before the matches start, so you don't miss any game of the Brazilian team.

## API

To facilitate the integration dynamics of our App, we created a Pseudo-API using GitHub Pages, which is available at the following URL: https://digitalinnovationone.github.io/copa-2022-android/api.json

## Project Challenge (Lab) 😎

1. :white_check_mark: Explore the base of the project and understand its modules and responsibilities:
    * **app**: Contains the application-level and scaffolding classes that tie the rest of the codebase together. The "app" module depends on all the required feature modules and core modules;
    * **data**: abstraction for accessing data sources, organized as follows:
        * ***data***: In this module the "remote" and "local" data sources are declared, as well as the implementation of the repositories according to the necessary business logic;
        * ***local***: Contains an implementation of [Room](https://developer.android.com/training/data-storage/room) as a local data source;
        * ***remote***: Implementation of a remote data source using [Retrofit](https://square.github.io/retrofit/) as an HTTP client.
    * **domain**: In this module the use cases (functionalities) of the application are declared;
    * **notification-scheduler**: Módulo específico para a criação das Notificações via Work Manager.
2. :white_check_mark: Specific module for creating Notifications via Work Manager.
    * Search Matches: `GetMatchesUseCase.kt`;
    * Enable Notification: `EnableNotificationUseCase.kt`;
    * Disabled Notification: `DisableNotificationUseCase.kt`.
3. :white_check_mark: Create MainViewModel.kt to orchestrate relaxants with MainActivity.kt;
4. :white_check_mark: Create MainScreen.kt to create a UI through Jetpack Compose;
5. :white_check_mark: Integrate ViewModel and Activity, through observation of states;
6. :white_check_mark: Finally, create Work Manager to orchestrate Push Notifications locally.


![Screenshot_20230702_000024](https://github.com/danhasegawa/copa-2022-android/assets/105471213/ee12fff2-49a1-4c82-855a-8633f00580d9)
