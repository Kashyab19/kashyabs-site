<script>
    export let profile;
  
    // Destructure profile object for easier use
    const { name, location, earnings, subscribers, newsletter } = profile;
  </script>
  
  <style>
    .profile-picture {
      border-radius: 50%;
      width: 100px;
      height: 100px;
    }
  
    .email-input {
      margin: 10px 0;
      padding: 10px;
      width: 80%;
      border: 1px solid #ddd;
      border-radius: 5px;
    }
  
    .subscribe-button {
      padding: 10px 20px;
      background-color: #ffa500;
      color: #fff;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
  
    .social-links {
      margin-top: 20px;
    }
  
    .social-links a {
      margin: 0 10px;
      color: #555;
      text-decoration: none;
    }
  
    .build-page-button {
      margin-top: 20px;
      padding: 10px 20px;
      background-color: #000;
      color: #fff;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
  </style>
  
  <!-- <img src="your-profile-image.jpg" alt="Profile Picture" class="profile-picture"> -->
  <h1>{name}</h1>
  <p>Location: {location}</p>
  <p>Monthly Earnings: {earnings}</p>
  <p>{subscribers} read <a href="#">{newsletter}:</a></p>
  <p>Your Saturday issue to find startup ideas, launch fast, and get profitable</p>
  <input type="email" placeholder="Your email..." class="email-input">
  <button class="subscribe-button">Subscribe</button>
  <div class="social-links">
    <a href="#">Twitter</a>
    <a href="#">LinkedIn</a>
    <a href="#">GitHub</a>
  </div>
  <button class="build-page-button">Build your Indie Page</button>
  