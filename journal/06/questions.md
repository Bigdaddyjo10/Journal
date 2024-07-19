# Single Page Applications with Vue
01. What is the entrypoint of an application?

  > | main.js |

02. What is the difference between a vue `component` and `page`?

  > | component reuses UI element, button, form. Used multiple times within an app focuses on specific functionality. page Represents a single view or screen tied to a route in the app contains multiple components |

03. What is ***Component-Based Architecture***?

  > | a software design approach that emphasizes building a system from smaller, reusable components |

04. What are the three tags that make up a Vue component?

  > | script template style |

05. What are ***lifecycle hooks***? What are lifecycle hooks used for?

  > | allow you to know when your component is created, added to the DOM, updated, or destroyed |

06. Which component in Vue does the vue-router use to mount pages onto?

  > | Vue Router uses the <router-view> component to mount pages onto |

07. What is the difference between the `AppState` and the state object within a component?

  > | Your AppState is global, and your component state is local.|

08. What is the responsibility of `Services` in our Vue projects?

  > | To handle the biasness logic |

09. What are ***props*** and how are they used? Provide an example

  > |Props are custom attributes you can register on a component. They are used to pass data from a parent component to a child component
  
  <script>
export default {
  props: {
    message: String
  }
};
</script>

   <template>
  <div>
    <p>{{ message }}</p>
  </div>
</template>

 |

10. What is the Vue method used to create watchable objects such as `state` or `AppState`?

  > | watchEffect | 