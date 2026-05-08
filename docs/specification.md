# 仕様

        ## 対象レコード

        - `guide`
- `step`
- `check`
- `evidence`

        ## 必須項目

        `title`, `step`, `nextAction`

        ## 警告項目

        `evidence`, `reviewDate`

        ## フロー

        1. 入力レコードを受け取る。
        2. `src/core/scenarioEngine.js` が必須項目と警告項目を評価する。
        3. `src/report/reportBuilder.js` が検証結果を集計する。
        4. `dist/validation-result.json` を release evidence の前提証跡にする。

        ## 保存方針

        スクリーンショットや個人環境名はサンプルに含めない
