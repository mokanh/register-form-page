<template>
  <div class="layout form-reg">
    <b-form>
      <b-form-group id="input-group-1" label="Name">
        <div class="row">
          <div class="col-md-6">
            <b-form-input label="First Name" required placeholder="First Name" class></b-form-input>
          </div>
          <div class="col-md-6">
            <b-form-input required placeholder="Last name" class></b-form-input>
          </div>
        </div>
      </b-form-group>
      <b-form-group label="Email">
        <b-form-input type="email" required placeholder="Email" class></b-form-input>
      </b-form-group>
      <b-form-group label="Password">
        <b-form-input type="password" required placeholder="Password" class></b-form-input>
      </b-form-group>
      <b-form-group label="Gender">
        <b-form-select :options="gender" required class></b-form-select>
      </b-form-group>
      <b-form-group label="City">
        <b-form-select :options="city" required></b-form-select>
      </b-form-group>

      <b-button type="submit" variant="secondary" class="btn-custom">Submit</b-button>
    </b-form>
  </div>
</template>
<script>
export default {
  data() {
    return {
      form: {
        email: "",
        name: "",
        gender: null
      },
      gender: ["Male", "Female"],
      city: [
        "Bandung",
        "Garut",
        "Ciamis",
        "Tasik",
        "Jakarta",
        "Surabaya",
        "Bogor",
        "Depok",
        "Bekasi",
        "Bangka"
      ],
      show: true
    };
  }
};
</script>
<style lang="scss">
.layout {
  max-width: 600px;
  margin: auto;
}
.btn-custom {
  display: block;
  width: 100%;
}
.form-reg {
  padding: 5rem 0;
  margin-top: -10rem;
  margin-bottom: 5rem;
  background: #fff;
  padding: 2rem;
  z-index: 9999;
  position: relative;
  box-shadow: 0px 0px 34px 0px rgba(0, 0, 0, 0.11);
}
.form-title {
  position: relative;
  &::after {
    content: "";
    width: 50%;
    height: 3px;
    background: indigo;
    position: absolute;
    bottom: -10px;
    left: 0;
    right: 0;
    margin: auto;
  }
}
@media (max-width: 900px) {
  .form-reg {
    margin-top: 2rem;
    margin-bottom: 2rem;
    box-shadow: none;
  }
}
</style>