<template>
    <div class="messagebar">
        <div class="messagebox">
            <img class="icon-message" width="12" height="12" src="~/assets/images/icon/Icon_bell.png">
            Messages
        </div>
        <div class="arrow"></div>
    </div>
</template>

<style>
.icon-message {
    filter: invert(100%);
    justify-self: end;
    align-self: center;
}

.messagebar {
    background-color: #676767;
    height: 40px;
    display: flex;
    justify-content: center;
    align-items: center;
}

.messagebox {
    background-color: #8766c4;
    color: white;
    text-align: center;
    border-radius: 4px;
    width: 150px;
    height: 24px;
}

.arrow {
    width: 0;
    height: 0;
    border-top: 5px solid transparent;
    border-bottom: 5px solid transparent;
    border-left: 5px solid #8766c4;
}
</style>