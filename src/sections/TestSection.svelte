<script>
  import Scroller from "../lib/Scroller.svelte";
  import ArticleText from "../lib/ArticleText.svelte";
</script>

<div>
  <Scroller layout="left">
    {#snippet sticky()}
      <h2>Homeownership Disparities in New Jersey</h2>
      <p>Visualizing rental trends, income burdens, and loan approvals by race.</p>
    {/snippet}

    {#snippet scrolly()}
      <ArticleText>
        <h3>Rental Vacancy Rates (2016–2025)</h3>
        <p>Rental vacancy rates have fluctuated in New Jersey, affecting housing availability.</p>
        <img src="/rental_vacancy.png" alt="Rental Vacancy Rates" width="600" />
      </ArticleText>

      <ArticleText>
        <h3>Percentage of Income Spent on Rent</h3>
        <p>Black households in Union County, NJ, spend 30.4% of their income on rent on average.</p>
        <img src="/percent_income_spent_rent.png" alt="Percent Income Spent on Rent" width="600" />
      </ArticleText>

      <ArticleText>
        <h3>Loan Originations (2023)</h3>
        <div style="display: flex; gap: 20px;">
          <div>
            <h4>Black or African American</h4>
            <img src="/loan_originated_black.png" alt="Loan Originations Black" width="280" />
          </div>
          <div>
            <h4>White</h4>
            <img src="/loan_originated_white.png" alt="Loan Originations White" width="280" />
          </div>
        </div>
      </ArticleText>

      <ArticleText>
        <h3>Loan Denials (2023)</h3>
        <div style="display: flex; gap: 20px;">
          <div>
            <h4>Black or African American</h4>
            <img src="/loan_denials_black.png" alt="Loan Denials Black" width="280" />
          </div>
          <div>
            <h4>White</h4>
            <img src="/loan_denials_white.png" alt="Loan Denials White" width="280" />
          </div>
        </div>
      </ArticleText>
    {/snippet}
  </Scroller>
</div>

