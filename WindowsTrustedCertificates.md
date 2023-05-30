## 要申請 Windows 應用程式的可信憑證，您需要遵循以下步驟：

1. 建立憑證要求（Certificate Signing Request, CSR）：
   - 開啟 Microsoft Management Console（MMC）。
   - 在左側的樹狀目錄中，展開「Certificates (Local Computer)」，然後選擇「Personal」>「Certificates」。
   - 在右側窗格中，右鍵點擊空白處，選擇「All Tasks」>「Advanced Operations」>「Create Custom Request...」。
   - 在「Certificate Enrollment」視窗中，選擇「Proceed without enrollment policy」，然後按「Next」。
   - 選擇「(No template) Legacy key」，然後按「Next」。
   - 在「Certificate Information」頁面上，選擇「Properties」。
   - 在「General」標籤中，輸入您的應用程式的通用名稱、組織名稱等資訊。
   - 在「Private Key」標籤中，選擇憑證的長度和其他相關設定。
   - 完成設定後，按「Next」。
   - 指定要保存 CSR 的檔案名稱和位置，然後按「Finish」。

2. 申請憑證：
   - 使用您選擇的憑證供應商的網站或系統，將您的 CSR 提交給他們。
   - 根據您的憑證供應商的要求，填寫相關的資訊並完成憑證申請程序。

3. 下載並安裝憑證：
   - 憑證供應商將向您提供已簽署的憑證，通常以 .cer 或 .pfx 格式提供。
   - 下載並保存這些憑證到您的電腦上。

4. 安裝憑證：
   - 開啟 Microsoft Management Console（MMC）。
   - 在左側的樹狀目錄中，展開「Certificates (Local Computer)」，然後選擇「Personal」>「Certificates」。
   - 在右側窗格中，右鍵點擊空白處，選擇「All Tasks」>「Import...」。
   - 在「Certificate Import Wizard」視窗中，按「Next」。
   - 瀏覽並選擇您下載的憑證檔案，然後按「Next」。
   - 根據需要，選擇要將憑證安裝到「Personal」憑證存儲區或其他
