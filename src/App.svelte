<script>
  import Header from "./components/header.svelte";
  import Kanban from "./kanban.svelte";
</script>

<Header />

<main>
  <div class="title">
    <span class="text1">Kan-Ban board</span>
    <span class="edit">
      <svg
        width="16"
        height="16"
        viewBox="0 0 16 16"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M9.71667 5.51667L10.4833 6.28333L2.93333 13.8333H2.16667V13.0667L9.71667 5.51667ZM12.7167 0.5C12.5083 0.5 12.2917 0.583333 12.1333 0.741667L10.6083 2.26667L13.7333 5.39167L15.2583 3.86667C15.5833 3.54167 15.5833 3.01667 15.2583 2.69167L13.3083 0.741667C13.1417 0.575 12.9333 0.5 12.7167 0.5ZM9.71667 3.15833L0.5 12.375V15.5H3.625L12.8417 6.28333L9.71667 3.15833Z"
          fill="#212529"
        />
      </svg>
    </span>
    <span class="adduser">
      <svg
        width="21"
        height="15"
        viewBox="0 0 21 15"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M13.3636 7.5C15.4732 7.5 17.1818 5.82188 17.1818 3.75C17.1818 1.67812 15.4732 0 13.3636 0C11.2541 0 9.54545 1.67812 9.54545 3.75C9.54545 5.82188 11.2541 7.5 13.3636 7.5ZM13.3636 1.875C14.4136 1.875 15.2727 2.71875 15.2727 3.75C15.2727 4.78125 14.4136 5.625 13.3636 5.625C12.3136 5.625 11.4545 4.78125 11.4545 3.75C11.4545 2.71875 12.3136 1.875 13.3636 1.875ZM13.3636 9.375C10.815 9.375 5.72727 10.6313 5.72727 13.125V15H21V13.125C21 10.6313 15.9123 9.375 13.3636 9.375ZM7.63636 13.125C7.84636 12.45 10.7959 11.25 13.3636 11.25C15.9409 11.25 18.9 12.4594 19.0909 13.125H7.63636ZM4.77273 10.3125V7.5H7.63636V5.625H4.77273V2.8125H2.86364V5.625H0V7.5H2.86364V10.3125H4.77273Z"
          fill="#171A21"
        />
      </svg>
    </span>
  </div>

  <div class="lists">
    <Kanban />
  </div>
</main>

<style>
  .title {
    position: absolute;
    /* width: auto;
    height: 39px; */ 
    /* commented by jsaha */
    left: 112px;
    top: 96px;
    /* added by jsaha */
    display: flex;
    justify-content: space-around;
  }

  .lists {
    position: absolute;
    width: auto;
    height: 482px;
    right: 0px;
    left: 112px;
    top: calc(50% - 482px / 2 + 39px);
  }

  .text1 {
    /* position: absolute;
    width: 371px;
    height: 39px; */
    /* commented by jsaha */

    /* Headline 2 */

    font-family: "Inter";
    font-style: normal;
    font-weight: 600;
    font-size: 32px;
    line-height: 39px;
    /* identical to box height */

    /* display: flex;
    align-items: flex-end; */
    /* commented by jsaha */
    letter-spacing: 0.384px;

    color: #171a21;
  }

  .edit {
    /* position: relative;
    width: 20px;
    height: 20px;
    left: 495px; */
    /* commented by jsaha */
    /* top: 93px; */
    /* Added by jsaha */
    margin-left: 10px;
    margin-top: 10px;
  }

  .adduser {
    position: absolute;
    /* left: 40.47%; */
    /* right: 57.89%; */
    left: 550px;
    top: 15.11%;
    bottom: 82.77%;

    background: #171a21;
  }

  .list {
    box-sizing: border-box;

    /* Auto layout */

    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 16px 4px;
    gap: 20px;

    position: absolute;
    width: 332px;
    top: 0px;

    border: 1px solid #d0d5dd;
    border-radius: 8px;
  }

  #list1 {
    height: 482px;
    left: 724px;
  }
  #list2 {
    height: 308px;
    left: 363px;
  }
  #list3 {
    height: 395px;
    left: 0px;
  }

  .addlist {
    box-sizing: border-box;

    /* Auto layout */

    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    padding: 8px 12px;
    gap: 4px;

    position: absolute;
    width: 141px;
    height: 36px;
    left: 1085px;
    top: 0px;

    /* Primary */

    background: #8447ff;
    /* Primary */

    border: 1px solid #8447ff;
    border-radius: 8px;
  }
</style>
