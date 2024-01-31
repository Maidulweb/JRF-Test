<script>
import ProfilePhoto from "../assets/Profile photo.png";
export default {
  data: function () {
    return {
      ProfilePhoto: ProfilePhoto,
    };
  },
};
</script>
<template>
  <div>
    <div class="information-accordion">
      <div class="accordion" id="accordionExample">
        <div class="d-flex justify-content-between information-accodion-header">
          <button
            class="information-accordion-btn"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#collapseOne"
            aria-controls="collapseOne"
          >
            Basic Information
          </button>
          <button
            class="information-accordion-btn"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#collapseTwo"
            aria-expanded="false"
            aria-controls="collapseTwo"
          >
            Education
          </button>
          <button
            class="information-accordion-btn"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#collapseThree"
            aria-expanded="false"
            aria-controls="collapseThree"
          >
            Work History
          </button>
          <button
            class="information-accordion-btn"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#collapseThree"
            aria-expanded="false"
            aria-controls="collapseThree"
          >
            Skills & Language
          </button>
          <button
            class="information-accordion-btn"
            type="button"
            data-bs-toggle="collapse"
            data-bs-target="#collapseThree"
            aria-expanded="false"
            aria-controls="collapseThree"
          >
            Portfolios & Certifications
          </button>
        </div>
        <div class="information-accordion-item">
          <div
            id="collapseOne"
            class="accordion-collapse collapse show"
            data-bs-parent="#accordionExample"
          >
            <div class="information-accordion-body">
              <div class="photo-resume">
                <div class="row">
                  <div class="col-md-6">
                    <div class="profile-photo">
                      <h6>Profile Photo</h6>

                      <form>
                        <fieldset class="upload_dropZone text-center mb-3 p-4">
                          <legend class="visually-hidden">
                            Image uploader
                          </legend>

                          <img :src="ProfilePhoto" />

                          <p class="small my-2">Profile photo max 2MB</p>

                          <input
                            id="upload_image_background"
                            class="position-absolute invisible"
                            type="file"
                            multiple
                            accept="image/jpeg, image/png, image/svg+xml"
                          />

                          <label
                            class="btn btn-upload mb-3"
                            for="upload_image_background"
                            >Choose file(s)</label
                          >
                        </fieldset>
                      </form>
                    </div>
                  </div>
                  <div class="col-md-6">
                    <div class="resume-upload">
                      <h6>Resume Upload</h6>
                      <p>English Resume</p>
                      <div class="form-group">
                        <label
                          for="file"
                          class="custom-file-label d-flex justify-content-between"
                        >
                          <span class="js-fileName">Add option</span>
                          <span>+</span>
                        </label>
                        <input
                          type="file"
                          name="file"
                          id="file"
                          class="custom-file"
                        />
                      </div>
                      <p>English Resume</p>
                      <div class="form-group">
                        <label
                          for="file"
                          class="custom-file-label d-flex justify-content-between"
                        >
                          <span class="js-fileName">Add option</span>
                          <span>+</span>
                        </label>
                        <input
                          type="file"
                          name="file"
                          id="file"
                          class="custom-file"
                        />
                      </div>
                      <p>English Resume</p>
                      <div class="form-group">
                        <label
                          for="file"
                          class="custom-file-label d-flex justify-content-between"
                        >
                          <span class="js-fileName">Add option</span>
                          <span>+</span>
                        </label>
                        <input
                          type="file"
                          name="file"
                          id="file"
                          class="custom-file"
                        />
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <div class="basic-information">
                <div class="d-flex justify-content-between">
                  <h5>Basic Information</h5>
                  <span>+</span>
                </div>
                <hr />
                <div class="basic-information-body">
                  <div class="row">
                    <div class="col-md-6">
                      <h6>First Name</h6>
                      <p>Nur</p>
                      <h6>First Name</h6>
                      <p>Nur</p>
                      <h6>First Name</h6>
                      <p>Nur</p>
                      <h6>First Name</h6>
                      <p>Nur</p>
                      <h6>First Name</h6>
                      <p>Nur</p>
                      <h6>First Name</h6>
                      <p>Nur</p>
                    </div>
                    <div class="col-md-6">
                      <h6>First Name</h6>
                      <p>Nur</p>
                      <h6>First Name</h6>
                      <p>Nur</p>
                      <h6>First Name</h6>
                      <p>Nur</p>
                      <h6>First Name</h6>
                      <p>Nur</p>
                      <h6>First Name</h6>
                      <p>Nur</p>
                    </div>
                  </div>
                </div>
              </div>
              <div class="address-information">
                <div class="d-flex justify-content-between">
                  <h5>Address Information</h5>
                  <span>+</span>
                </div>
                <hr />
                <div class="address-information-body">
                  <div class="row">
                    <div class="col-md-4">
                      <h6>First Name</h6>
                    </div>
                    <div class="col-md-8">
                      <p>First Name</p>
                    </div>
                  </div>
                  <div class="row">
                    <div class="col-md-4">
                      <h6>First Name</h6>
                    </div>
                    <div class="col-md-8">
                      <p>First Name</p>
                    </div>
                  </div>
                  <div class="row">
                    <div class="col-md-4">
                      <h6>First Name</h6>
                    </div>
                    <div class="col-md-8">
                      <p>First Name</p>
                    </div>
                  </div>
                  <div class="row">
                    <div class="col-md-4">
                      <h6>First Name</h6>
                    </div>
                    <div class="col-md-8">
                      <p>First Name</p>
                    </div>
                  </div>
                  <div class="row">
                    <div class="col-md-4">
                      <h6>First Name</h6>
                    </div>
                    <div class="col-md-8">
                      <p>First Name</p>
                    </div>
                  </div>
                  <div class="row">
                    <div class="col-md-4">
                      <h6>First Name</h6>
                    </div>
                    <div class="col-md-8">
                      <p>First Name</p>
                    </div>
                  </div>
                </div>
              </div>
              <div class="social-profile">
                <div class="d-flex justify-content-between">
                  <h5>Social Profile</h5>
                  <span>+</span>
                </div>
                <hr />
                <div class="basic-information-body">
                  <div class="row">
                    <div class="col-md-6">
                      <h6>Facebook</h6>
                      <p>Nur</p>
                      <h6>Twitter</h6>
                      <p>Nur</p>
                    </div>
                    <div class="col-md-6">
                      <h6>Linkedin</h6>
                      <p>Nur</p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="accordion-item">
          <div
            id="collapseTwo"
            class="accordion-collapse collapse"
            data-bs-parent="#accordionExample"
          >
            <div class="accordion-body">
              <strong>This is the second item's accordion body.</strong> It is
              hidden by default, until the collapse plugin adds the appropriate
              classes that we use to style each element. These classes control
              the overall appearance, as well as the showing and hiding via CSS
              transitions. You can modify any of this with custom CSS or
              overriding our default variables. It's also worth noting that just
              about any HTML can go within the <code>.accordion-body</code>,
              though the transition does limit overflow.
            </div>
          </div>
        </div>
        <div class="accordion-item">
          <div
            id="collapseThree"
            class="accordion-collapse collapse"
            data-bs-parent="#accordionExample"
          >
            <div class="accordion-body">
              <strong>This is the third item's accordion body.</strong> It is
              hidden by default, until the collapse plugin adds the appropriate
              classes that we use to style each element. These classes control
              the overall appearance, as well as the showing and hiding via CSS
              transitions. You can modify any of this with custom CSS or
              overriding our default variables. It's also worth noting that just
              about any HTML can go within the <code>.accordion-body</code>,
              though the transition does limit overflow.
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<style>
.information-accodion-header {
  background: #fff;
  padding: 20px 0;
}
.information-accordion-btn {
  border: 0;
  background: transparent;
  font-size: 14px;
  line-height: 19.36px;
}
.resume-upload p {
  padding-bottom: 0;
  margin-bottom: 0;
}
.custom-file {
  opacity: 0;
  overflow: hidden;
  width: 0;
  height: 0;
  z-index: -1;
}
.custom-file-label {
  background: #b3b1b1;
  height: 100%;
}
</style>
