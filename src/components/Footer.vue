<template>
  <div class="container">
    <div class="row">
      <div class="col-12 col-lg-3">
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
        <div class="collapse multi-collapse" id="multiCollapseExample1">
          <div class="card card-body">
            Some placeholder content for the first collapse component of this
            multi-collapse example. This panel is hidden by default but revealed
            when the user activates the relevant trigger.
          </div>
        </div>
      </div>

      <div class="col-12 col-lg-3">
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
        <div class="collapse multi-collapse" id="multiCollapseExample2">
          <div class="card card-body">
            Some placeholder content for the second collapse component of this
            multi-collapse example. This panel is hidden by default but revealed
            when the user activates the relevant trigger.
          </div>
        </div>
      </div>

      <div class="col-12 col-lg-3">
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
        <div class="collapse multi-collapse" id="multiCollapseExample3">
          <div class="card card-body">
            Some placeholder content for the second collapse component of this
            multi-collapse example. This panel is hidden by default but revealed
            when the user activates the relevant trigger.
          </div>
        </div>
      </div>
      <div class="col-12 col-lg-3">
        <div class="card">
          <div class="card-body">
            <h5 class="card-title">Card title</h5>
            <h6 class="card-title">Card subtitle</h6>
            <form>
              <div class="form-floating mb-3">
                <input
                  type="email"
                  class="form-control"
                  id="floatingInput"
                  placeholder="name@example.com"
                />
                <label for="floatingInput">Email address</label>
              </div>
              <div class="form-check">
                <input
                  class="form-check-input"
                  type="checkbox"
                  id="gridCheck1"
                />
                <label class="form-check-label" for="gridCheck1">
                  Example checkbox
                </label>
              </div>
            </form>
          </div>
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
