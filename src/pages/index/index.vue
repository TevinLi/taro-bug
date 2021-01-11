<template>
    <view class="index">
        <view>
            <view>checkbox disabled 无效</view>
            <label>
                <checkbox disabled>测试</checkbox>
                <checkbox :disabled="true">测试</checkbox>
            </label>
        </view>
        <view>
            <view>checkbox group disabled 无效</view>
            <checkbox-group @change="evt=>null">
                <label>
                    <checkbox
                        :value="1"
                        :disabled="true"
                    >组测试1
                    </checkbox>
                </label>
                <label>
                    <checkbox
                        :value="2"
                        :disabled="false"
                    >组测试1
                    </checkbox>
                </label>
            </checkbox-group>
        </view>
    </view>
</template>

<script>
import './index.scss';

export default {
    data() {
        return {
            msg: 'Hello world!',
        };
    },
};
</script>
