<template>
  <div class="container">
    <div class="row">
      <p>
        <a
          class="btn btn-primary"
          data-bs-toggle="collapse"
          href="#multiCollapseExample1"
          role="button"
          aria-expanded="false"
          aria-controls="multiCollapseExample1"
          >Toggle element 1</a
        >
      </p>
      <div class="col">
        <div class="collapse multi-collapse" id="multiCollapseExample1">
          <div class="card card-body">
            Some placeholder content for the first collapse component of this
            multi-collapse example. This panel is hidden by default but revealed
            when the user activates the relevant trigger.
          </div>
        </div>
      </div>
      <p>
        <button
          class="btn btn-primary"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#multiCollapseExample2"
          aria-expanded="false"
          aria-controls="multiCollapseExample2"
        >
          Toggle element 2
        </button>
      </p>
      <div class="col">
        <div class="collapse multi-collapse" id="multiCollapseExample2">
          <div class="card card-body">
            Some placeholder content for the second collapse component of this
            multi-collapse example. This panel is hidden by default but revealed
            when the user activates the relevant trigger.
          </div>
        </div>
      </div>
      <p>
        <button
          class="btn btn-primary"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#multiCollapseExample3"
          aria-expanded="false"
          aria-controls="multiCollapseExample3"
        >
          Toggle element 3
        </button>
      </p>
      <div class="col">
        <div class="collapse multi-collapse" id="multiCollapseExample3">
          <div class="card card-body">
            Some placeholder content for the second collapse component of this
            multi-collapse example. This panel is hidden by default but revealed
            when the user activates the relevant trigger.
          </div>
        </div>
      </div>
    </div>
    <div class="card" style="width: 18rem">
      <div class="card-body">
        <h5 class="card-title">Card title</h5>
        <h6 class="card-title">Card subtitle</h6>
        <div class="mb-3">
          <input
            type="email"
            class="form-control"
            id="exampleFormControlInput1"
            placeholder="name@example.com"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
  props: {
    title: String,
  },
};
</script>
