<style lang="postcss">

</style>
<!-- Todos.svelte -->
<div class="container mx-auto">
    <!-- NewTodo -->
    <div class="container mx-auto">
    <form>
      <h1 class="text-2xl text-center mb-4 mt-8">
        <label for="todo-0"> What needs to be done? </label>
      </h1>
      <input type="text" id="todo-0" autocomplete="off" class="p-4 border-black border-solid border-2 w-full" />
      <button type="submit" disabled="" class="text-2xl my-4 p-2 rounded-lg bg-cyan-400 hover:bg-cyan-500 w-full">
        Add
      </button>
    </form>
    </div>
  
    <!-- Filter -->
    <div class="ontainer mx-auto">
      <button class="btn toggle-btn" aria-pressed="true">
        <span class="visually-hidden">Show</span>
        <span>All</span>
        <span class="visually-hidden">tasks</span>
      </button>
      <button class="btn toggle-btn" aria-pressed="false">
        <span class="visually-hidden">Show</span>
        <span>Active</span>
        <span class="visually-hidden">tasks</span>
      </button>
      <button class="btn toggle-btn" aria-pressed="false">
        <span class="visually-hidden">Show</span>
        <span>Completed</span>
        <span class="visually-hidden">tasks</span>
      </button>
    </div>
  
    <!-- TodosStatus -->
    <h2 class="text-3xl font-extrabold text-start mb-6 mt-4">2 out of 3 items completed</h2>
  
    <!-- Todos -->
    <ul role="list" class="container mx-auto" aria-labelledby="list-heading">
      <!-- todo-1 (editing mode) -->
      <li class="todo">
        <div class="stack-small">
          <form class="stack-small">
            <div class="form-group">
              <label for="todo-1" class="todo-label">
                New name for 'Create a Svelte starter app'
              </label>
              <input
                type="text"
                id="todo-1"
                autocomplete="off"
                class="todo-text" />
            </div>
            <div class="btn-group">
              <button class="btn todo-cancel" type="button">
                Cancel
                <span class="visually-hidden">renaming Create a Svelte starter app</span>
              </button>
              <button class="btn btn__primary todo-edit" type="submit">
                Save
                <span class="visually-hidden">new name for Create a Svelte starter app</span>
              </button>
            </div>
          </form>
        </div>
      </li>
  
      <!-- todo-2 -->
      <li class="todo">
        <div class="stack-small">
          <div class="c-cb">
            <input type="checkbox" id="todo-2" checked />
            <label for="todo-2" class="todo-label">
              Create your first component
            </label>
          </div>
          <div class="btn-group">
            <button type="button" class="btn">
              Edit
              <span class="visually-hidden">Create your first component</span>
            </button>
            <button type="button" class="btn btn__danger">
              Delete
              <span class="visually-hidden">Create your first component</span>
            </button>
          </div>
        </div>
      </li>
  
      <!-- todo-3 -->
      <li class="todo">
        <div class="stack-small">
          <div class="c-cb">
            <input type="checkbox" id="todo-3" />
            <label for="todo-3" class="todo-label">
              Complete the rest of the tutorial
            </label>
          </div>
          <div class="btn-group">
            <button type="button" class="btn">
              Edit
              <span class="visually-hidden">Complete the rest of the tutorial</span>
            </button>
            <button type="button" class="btn btn__danger">
              Delete
              <span class="visually-hidden">Complete the rest of the tutorial</span>
            </button>
          </div>
        </div>
      </li>
    </ul>
    
    <!-- MoreActions -->
    <div class="btn-group">
      <button type="button" class="btn btn__primary">Check all</button>
      <button type="button" class="btn btn__primary">Remove completed</button>
    </div>
  </div>
  
