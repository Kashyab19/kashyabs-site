<script>
    export let projects;
  </script>
  
  <style>
    .project-card {
      background-color: #fff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
    }
  
    .project-card h2 {
      margin: 10px 0;
    }
  
    .project-card p {
      margin: 5px 0;
    }
  </style>
  
  {#each projects as project}
    <div class="project-card">
      <h2>{project.title}</h2>
      <p>{project.description}</p>
      <p>{project.earnings}</p>
    </div>
  {/each}
  