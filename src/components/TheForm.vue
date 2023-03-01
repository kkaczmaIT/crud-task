<template>
    <div id="form">
        <form class="form">
            <h3 class="hfs-md fw-lg white-color d-flex justify-content-center">Campaign form</h3>
            <div class="form-input-group">
                <label for="campaignNameInput" class="form-label">Campaign name</label>
                <input type="text" class="form-input" id="campaignNameInput" placeholder="Enter campaign name" required>
            </div>
            <div class="form-input-group">
                <label for="keywordsInput" class="form-label">Keywords of product</label>
                <input type="text" class="form-input" id="keywordsInput" placeholder="Enter keywords" required>
            </div>
            <div class="form-input-group">
                <label for="bidAmountInput" class="form-label">Amount</label>
                <input type="number" class="form-input" id="bidAmountInput" placeholder="Enter bid amount" required>
            </div>
            <div class="form-input-group">
                <label for="campaignFundInput" class="form-label"></label>
                <input type="number" class="form-input" id="campaignFundInput" placeholder="Enter campaign fund" required>
            </div>
            <div class="form-input-group">
                <label class="form-label">Status</label>
                <div class="form-check-group">
                    <input type="checkbox" value="isOn" id="statusInput" required>
                    <label class="form-check-label" for="statusInput">
                        On 
                    </label>
                </div>
            </div>
            <div class="form-input-group">
                <label for="townsInput" class="form-label">Datalist example</label>
                <input class="form-input" list="townsList" id="townsInput" placeholder="Enter town name" required>
                <datalist id="townsList" class="form-input">
                    <option value="San Francisco" />
                    <option value="New York" />
                    <option value="Seattle" />
                    <option value="Los Angeles" />
                    <option value="Chicago" />
                </datalist>
            </div>

            <div class="form-input-group">
                <label for="radiusAmountInput" class="form-label">Radius (in kilometers)</label>
                <input type="number" class="form-input" id="radiusAmountInput" placeholder="Enter radius (km)" required>
            </div> 

            <!-- <div class="form-input-group">
                <label for="mySelect" class="form-label">Select example</label>
                <select class="form-select" id="mySelect" aria-label="Default select example">
                <option selected>Open this select menu</option>
                <option value="1">One</option>
                <option value="2">Two</option>
                <option value="3">Three</option>
                </select>
            </div>
            <div class="form-input-group">
                <label for="mySelect" class="form-label">Checkbox example</label>
                <div class="form-check-group">
                <input type="checkbox" value="" id="flexCheckDefault">
                <label class="form-check-label" for="flexCheckDefault">
                    Default checkbox
                </label>
                </div>
            </div> -->
            
            <div class="mt-1 d-flex align-items-center justify-content-center">
                <input type="submit" value="Add" class="btn btn-additional pr-3 pl-3 fs-lg" />
            </div>

        
        </form>
    </div>
</template>

<script>
    export default {
        name: 'TheForm'
    }
</script>

<style lang="scss">
    @import '@/assets/scss/global';

    #form {
        padding: 10%;
    }
</style>