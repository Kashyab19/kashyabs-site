<script>
    import Profile from '../components/Profile.svelte';
    import ProjectList from '../components/ProjectsList.svelte';
    
    // Sample data
    export let profile = {
      name: "Kashyab",
      location: "Your Location",
      earnings: "$xx,xxx/month",
      subscribers: "20,000+ solopreneurs",
      newsletter: "Just Ship It"
    };
  
    export let projects = [
      { title: "ShipFast", description: "Ship your startup in days, not months", earnings: "$77.9k/mo" },
      { title: "Indie Page", description: "All your startups in a page, like this one", earnings: "$1.7k/mo" },
      { title: "Zenvoice", description: "Focus on your startup, not the invoices", earnings: "$946/mo" },
      { title: "PoopUp", description: "Turn your visitors into customers with wake-up call", earnings: "$523/mo" },
      { title: "ByeDispute", description: "Prevent disputes before getting banned from Stripe", earnings: "$407/mo" },
      { title: "WorkbookPDF", description: "Language workbooks you'll love", earnings: "$19/mo" }
      // Add more projects as needed
    ];
  </script>
  
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      height: 100vh;
      background-color: #f0f0f0;
      display: flex;
      justify-content: center;
      align-items: center;
    }
  
    .container {
      display: flex;
      width: 80%;
      height: 90%;
      background-color: #fff;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
      border-radius: 10px;
      overflow: hidden;
    }
  
    .left-section {
      width: 300px;
      padding: 20px;
      background-color: #f9f9f9;
      box-shadow: 2px 0 5px rgba(0, 0, 0, 0.1);
      border-radius: 10px 0 0 10px;
      margin-right: 20px;
    }
  
    .right-section {
      flex-grow: 1;
      padding: 20px;
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
      gap: 20px;
      overflow-y: auto;
      height: 100%;
    }
  </style>
  
  <div class="container">
    <div class="left-section">
      <Profile {profile} />
    </div>
    <div class="right-section">
      <ProjectList {projects} />
    </div>
  </div>
  