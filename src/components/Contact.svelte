<script>
    import SparkleText from "./SparkleText.svelte";
    let name = '';
    let email = '';
    let Company = '';
    let message = '';
    const reset = () => {
        name = '';
        email = '';
        Company = '';
        message = '';
    }
    const sendMessage = () => {
        if (name === '' || email === '' || Company === '' || message === '') {
            alert('Please fill all the fields');
        } else {
            window.location.href = `mailto:darzhz@protonmail.com?subject=Contact from ${name}&body=${message}`;
            reset();
        }
    }
</script>
<h1>Contact Me</h1>
<div class="contain">
  <div class="wrapper">
    <div class="form">
      <h4>GET IN TOUCH</h4>
      <h2 class="form-headline">Ping me an email</h2>
      <div id="submit-form">
        <p>
          <input
            id="name"
            class="form-input"
            type="text"
            placeholder="Your Name*"
            bind:value={name}
          />
          <small class="name-error"></small>
        </p>
        <p>
          <input
            id="email"
            class="form-input"
            type="email"
            placeholder="Your Email*"
            bind:value={email}
          />
          <small class="name-error"></small>
        </p>
        <p class="full-width">
          <input
            id="company-name"
            class="form-input"
            type="text"
            placeholder="Company Name*"
            bind:value={Company}
            required
          />
          <small></small>
        </p>
        <p class="full-width">
          <textarea
            minlength="20"
            id="message"
            cols="30"
            rows="7"
            placeholder="Your Message*"
            bind:value={message}
            required
          ></textarea>
          <small></small>
        </p>
        <p class="full-width">
          <button
            type="submit"
            class="submit-btn"
            value="Submit"
            on:click={() => {
              sendMessage();
            }}
          >Send</button>
          <button class="reset-btn" on:click={()=>{reset()}}>Reset</button>
        </p>
      </div>
    </div>

    <div class="contacts contact-wrapper">
      <SparkleText fontSize={'2rem'}>Let's Build Something Great<br></SparkleText>
    </div>
  </div>
</div>
<div class="footer">
    <p>© 2024 Darsh Shyam Kumar</p>
</div>

<style>
    :root {
    --primary-color: #f5f5f531;
    }
    input, textarea{
        font-family: 'satoshi-light',sans-serif;
        color: white;
        outline: none;
    }
  .contain {
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: "satoshi-regular", sans-serif;
    color: white;
    margin: 30px 0px;
  }
  h1 {
    font-size: 2rem;
    font-weight: 700;
    text-align: center;
    margin: 0;
  }
  .wrapper {
    display: flex;
    justify-content: space-between;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    border-radius: 10px;
    width: 95%;
    box-shadow: 0 8px 32px 0 rgba(135, 78, 31, 0.37);
    backdrop-filter: blur(4px);
    -webkit-backdrop-filter: blur(4px);
    border-radius: 10px;
  }

  .form {
    width: 50%;
    padding: 20px;
  }

  .form-headline {
    margin: 0;
    font-size: 2rem;
    font-weight: 700;
    /* color: #333; */
  }

  .form-input,textarea {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border: 1px solid white;
    border-radius: 10px;
    background-color: var(--primary-color);
  }
  .form-input::placeholder {
    color: white;
  }
  textarea::placeholder {
    color: white;
  }
  /*   
    .full-width {
      width: 100%;
    } */

  textarea {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border-radius: 10px;
  }

  button {
        padding: 0.5rem 1rem;
        border: none;
        border-radius: 5px;
        background: rgba(255, 255, 255, 0.1);
        color: white;
        cursor: pointer;
        font-family: 'satoshi-light', sans-serif;
    }
    button:hover {
        background: rgba(255, 255, 255, 0.2);
    }
    button:active {
        background: rgba(255, 255, 255, 0.3);
    }
    button:focus {
        outline: none;
    }
    button:active {
        transform: scale(0.95);
    }
    button {
        transition: all 0.3s ease;
    }

  .contacts {
    width: 50%;
    padding: 20px;
    /* background-color: #f5f5f5; */
  }

  .contact-wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: black;
    border-radius: 15px;
  }
  .footer {
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #00000021;
    color: white;
    font-family: 'satoshi-regular', sans-serif;
    font-size: 1rem;
    padding: 10px;
  }
  @media (max-width: 768px) {
    .wrapper {
      flex-direction: column;
    }
    .form {
      width: 100%;
    }
    .contacts {
      width: 100%;
    }
  }
  @media (min-width: 1200px){
    .contain {
      width: 70vw;
      margin-left: auto;
      margin-right: auto;
    }
  }
  
</style>
