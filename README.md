# IPC_Without_Binding-Android-
Simple IPC in Android using handler and messenger.

#How I achieved?
Here are two different application:
1)MyService-->MyService is just a plain Service.
2)MyIpcActivity-->MyIpcActivity is an activity which has a handler.

We wrapped the handler to a messenger in the activity. We create a bundle in which we put the binder of the messenger which is wrapped from handler. Now we set an action to the intent and start the service. In service we catch that action and show a toast and we receive the messenger instance from the bundle and communicate back to the service.

#How to use?
Just download the source. Run MyService source and then run MyIpcActivity code.
