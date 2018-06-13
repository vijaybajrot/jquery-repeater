# jquery-repeater

#### Basic jQuery Repeater

jQuery Repeater is a basic repeater depends on jquery 2.* or above.

## Usage
**Html**
```html
<!-- Repeater Html Start -->
<div id="repeater">
    <!-- Repeater Heading -->
    <div class="repeater-heading">
        <h5 class="pull-left">Repeater</h5>
        <button class="btn btn-primary pt-5 pull-right repeater-add-btn">
            Add
        </button>
    </div>
    <div class="clearfix"></div>
    <!-- Repeater Items -->
    <div class="items" data-group="test">
        <!-- Repeater Item Content -->
        <div class="item-content">
            <div class="form-group">
                <label for="inputEmail" class="col-lg-2 control-label">Name</label>
                <div class="col-lg-10">
                    <input type="text" class="form-control" id="inputName" placeholder="Name" data-name="name">
                </div>
            </div>
            <div class="form-group">
                <label for="inputEmail" class="col-lg-2 control-label">Email</label>
                <div class="col-lg-10">
                    <input type="text" class="form-control" id="inputEmail" placeholder="Email" data-skip-name="true" data-name="email">
                </div>
            </div>
        </div>
        <!-- Repeater Remove Btn -->
        <div class="pull-right repeater-remove-btn">
            <button class="btn btn-danger remove-btn">
                Remove
            </button>
        </div>
        <div class="clearfix"></div>
    </div>
</div>
<!-- Repeater End -->
```


**Javascript**
```javascript
$("#repeater").createRepeater({
    showFirstItemToDefault: true,
});
```