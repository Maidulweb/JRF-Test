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
      <div class="d-flex justify-content-between information-accodion-header">
        <button class="information-accordion-btn active" type="button">
          Basic Information
        </button>
        <button class="information-accordion-btn" type="button">
          Education
        </button>
        <button class="information-accordion-btn" type="button">
          Work History
        </button>
        <button class="information-accordion-btn" type="button">
          Skills & Language
        </button>
        <button class="information-accordion-btn" type="button">
          Portfolios & Certifications
        </button>
      </div>
      <div class="information-accordion-item">
        <div>
          <div class="information-accordion-body">
            <div class="photo-resume">
              <div class="row">
                <div class="col-md-6">
                  <div class="profile-photo">
                    <h4>Profile Photo</h4>
                    <div class="profile-photo-form">
                      <form>
                        <fieldset class="upload_dropZone text-center">
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
                            class="profile-photo-upload-btn"
                            for="upload_image_background"
                            >Choose file(s)</label
                          >
                        </fieldset>
                      </form>
                    </div>
                  </div>
                </div>
                <div class="col-md-6">
                  <div class="resume-upload">
                    <h4>Resume Upload</h4>
                    <div class="all-resume-upload">
                      <h6>English Resume</h6>
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
                      <h6>Japanese Resume</h6>
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
                      <h6>Japanese Work History</h6>
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
            </div>
            <div class="basic-information">
              <div
                class="d-flex justify-content-between basic-information-header"
              >
                <h4 class="mb-0">Basic Information</h4>
                <div>
                  <!-- Button trigger modal -->
                  <button
                    type="button"
                    class="btn btn-primary basic-modal-btn"
                    data-bs-toggle="modal"
                    data-bs-target="#exampleModal"
                  >
                    <i class="fa-solid fa-pen-to-square"></i>
                  </button>

                  <!-- Modal -->
                  <div
                    class="modal fade"
                    id="exampleModal"
                    tabindex="-1"
                    aria-labelledby="exampleModalLabel"
                    aria-hidden="true"
                  >
                    <div class="modal-dialog">
                      <div class="modal-content">
                        <div class="modal-header">
                          <h5 class="modal-title" id="exampleModalLabel">
                            Basic Information
                          </h5>
                        </div>
                        <div class="modal-body">
                          <form class="row g-3">
                            <div class="col-md-6">
                              <label for="inputEmail4" class="form-label"
                                >First Name</label
                              >
                              <input
                                type="text"
                                class="form-control"
                                id="inputEmail4"
                                placeholder="Type Your First Name"
                              />
                            </div>
                            <div class="col-md-6">
                              <label for="inputPassword4" class="form-label"
                                >Password</label
                              >
                              <input
                                type="text"
                                class="form-control"
                                id="inputPassword4"
                                placeholder="Type Your Last Name"
                              />
                            </div>
                            <div class="col-md-6">
                              <label for="inputEmail4" class="form-label"
                                >First Name</label
                              >
                              <input
                                type="text"
                                class="form-control"
                                id="inputEmail4"
                                placeholder="Type Your First Name"
                              />
                            </div>
                            <div class="col-md-6">
                              <label for="inputPassword4" class="form-label"
                                >Password</label
                              >
                              <input
                                type="text"
                                class="form-control"
                                id="inputPassword4"
                                placeholder="Type Your Last Name"
                              />
                            </div>
                            <div class="col-md-6">
                              <label for="inputEmail4" class="form-label"
                                >First Name</label
                              >
                              <input
                                type="text"
                                class="form-control"
                                id="inputEmail4"
                                placeholder="Type Your First Name"
                              />
                            </div>
                            <div class="col-md-6">
                              <label for="inputPassword4" class="form-label"
                                >Password</label
                              >
                              <input
                                type="text"
                                class="form-control"
                                id="inputPassword4"
                                placeholder="Type Your Last Name"
                              />
                            </div>

                            <div
                              class="col-12 d-flex align-content-center justify-content-center gap-4"
                            >
                              <button
                                type="button"
                                class="btn btn-secondary"
                                data-bs-dismiss="modal"
                              >
                                Close
                              </button>
                              <button type="submit" class="btn btn-primary">
                                Sign in
                              </button>
                            </div>
                          </form>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
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
              <div
                class="d-flex justify-content-between address-information-header"
              >
                <h4>Address Information</h4>
                <div>
                  <!-- Button trigger modal -->
                  <button
                    type="button"
                    class="btn btn-primary address-modal-btn"
                    data-bs-toggle="modal"
                    data-bs-target="#address"
                  >
                    <i class="fa-solid fa-pen-to-square"></i>
                  </button>

                  <!-- Modal -->
                  <div
                    class="modal fade"
                    id="address"
                    tabindex="-1"
                    aria-labelledby="exampleModalLabel"
                    aria-hidden="true"
                  >
                    <div class="modal-dialog">
                      <div class="modal-content">
                        <div class="modal-header">
                          <h5 class="modal-title" id="exampleModalLabel">
                            Address Information
                          </h5>
                        </div>
                        <div class="modal-body">
                          <form class="row g-3">
                            <div class="col-md-6">
                              <label for="inputEmail4" class="form-label"
                                >Email</label
                              >
                              <input
                                type="email"
                                class="form-control"
                                id="inputEmail4"
                              />
                            </div>
                            <div class="col-md-6">
                              <label for="inputPassword4" class="form-label"
                                >Password</label
                              >
                              <input
                                type="password"
                                class="form-control"
                                id="inputPassword4"
                              />
                            </div>

                            <div class="col-12">
                              <button
                                type="button"
                                class="btn btn-secondary"
                                data-bs-dismiss="modal"
                              >
                                Close
                              </button>
                              <button type="submit" class="btn btn-primary">
                                Sign in
                              </button>
                            </div>
                          </form>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
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
            <div class="social-information">
              <div
                class="d-flex justify-content-between social-information-header"
              >
                <h4>Social Profile</h4>
                <div>
                  <!-- Button trigger modal -->
                  <button
                    type="button"
                    class="btn btn-primary social-modal-btn"
                    data-bs-toggle="modal"
                    data-bs-target="#social"
                  >
                    <i class="fa-solid fa-pen-to-square"></i>
                  </button>

                  <!-- Modal -->
                  <div
                    class="modal fade"
                    id="social"
                    tabindex="-1"
                    aria-labelledby="exampleModalLabel"
                    aria-hidden="true"
                  >
                    <div class="modal-dialog">
                      <div class="modal-content">
                        <div class="modal-header">
                          <h5 class="modal-title" id="exampleModalLabel">
                            Social Profiles
                          </h5>
                        </div>
                        <div class="modal-body">
                          <form class="row g-3">
                            <div class="col-md-6">
                              <label for="inputEmail4" class="form-label"
                                >Email</label
                              >
                              <input
                                type="email"
                                class="form-control"
                                id="inputEmail4"
                              />
                            </div>
                            <div class="col-md-6">
                              <label for="inputPassword4" class="form-label"
                                >Password</label
                              >
                              <input
                                type="password"
                                class="form-control"
                                id="inputPassword4"
                              />
                            </div>

                            <div class="col-12">
                              <button
                                type="button"
                                class="btn btn-secondary"
                                data-bs-dismiss="modal"
                              >
                                Close
                              </button>
                              <button type="submit" class="btn btn-primary">
                                Sign in
                              </button>
                            </div>
                          </form>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <div class="social-information-body">
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
    </div>
  </div>
</template>
<style>
.information-accodion-header {
  background: #fff;
  margin: 30px 0;
  padding: 0 5px;
}
.information-accordion-btn {
  border: 0;
  border-right: 1px solid #e7e4e4;
  background: transparent;
  font-size: 14px;
  line-height: 19.36px;
  position: relative;
  padding: 10px 15px;
  margin: 8px 0;
}
.information-accordion-btn.active,
.information-accordion-btn:hover {
  border: 1px solid #e7e4e4;
  box-shadow: 1px 1px 11px 4px #e7e4e4;
  border-radius: 8px;
  background: #fff;
  color: #bd202e;
  font-weight: 600;
}
.information-accordion-btn:last-child {
  border-right: 0;
}
.profile-photo,
.resume-upload {
  background: #fff;
  border-radius: 8px;
}
.profile-photo h4,
.resume-upload h4 {
  border-bottom: 2px solid #d9d9d9;
  padding: 20px 0 10px 20px;
}
.profile-photo-form {
  padding: 5px 20px 15px 20px;
}
.profile-photo-form form {
  border: 1px dotted #be1e2d;
  padding: 20px;
  background-color: #fff5f5;
  border-radius: 8px;
}
.profile-photo-upload-btn {
  background: #bd202e;
  border: 1px solid #bd202e;
  padding: 8px 40px;
  border-radius: 8px;
  color: #fff;
  font-size: 18px;
  font-weight: 500;
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
  padding: 8px 10px;
  border-radius: 4px;
}
.form-group {
  margin-bottom: -3px;
}
.all-resume-upload {
  padding: 6px 20px;
}
/* Basic Information */

.basic-information,
.address-information,
.social-information {
  margin-top: 30px;
  background: #fff;
  border-radius: 8px;
}
.basic-information-header,
.address-information-header,
.social-information-header {
  border-bottom: 2px solid #d9d9d9;
  padding: 20px 25px;
}
.basic-information-header .basic-modal-btn,
.address-information-header .address-modal-btn,
.social-information-header .social-modal-btn {
  background: transparent;
  border: 0;
  color: #bd202e;
}
.btn-close {
  color: #bd202e !important;
}
.basic-information-header button:hover,
.address-information-header button:hover,
.social-information-header button:hover {
  background: transparent;
  border: 0;
  color: #bd202e;
}
.basic-information-header button i,
.address-information-header button i,
.social-information-header button i {
  color: #be1e2d;
}

.basic-information-body,
.address-information-body,
.social-information-body {
  padding: 20px 0 10px 20px;
}
.basic-information-body h6,
.address-information-body h6,
.social-information-body h6 {
  font-weight: 600;
}
</style>
