<span data-ttu-id="0f217-p119">電子メールを作成するために、コードはセッション トークンからユーザー名と、フォームから渡されたパラメーターから受信者の電子メール アドレスを取得します。次に、コードはプロジェクトに含まれるテンプレートから電子メールの本文を読み取り、ユーザー名と電子メール アドレスを補間し、HTTP 要求の本文として電子メールのテキストを添付します。</span><span class="sxs-lookup"><span data-stu-id="0f217-p119">To create the email, the code pulls the user name from the session token and the recipient email address from the parameters passed from the form. The code then reads the email body from a template included in the project, interpolates the user name and email address, and attaches the email text as the HTTP request body.</span></span>

電子メールを作成するために、コードはセッション トークンからユーザー名と、フォームから渡されたパラメーターから受信者の電子メール アドレスを取得します。次に、コードはプロジェクトに含まれるテンプレートから電子メールの本文を読み取り、ユーザー名と電子メール アドレスを補間し、HTTP 要求の本文として電子メールのテキストを添付します。

<span data-ttu-id="0f217-194">電子メールを送信するために、コードは HTTP 要求を作成し、認証ヘッダーとしてアクセス トークンを添付し、電子メール送信のエンドポイントに要求を投稿します。</span><span class="sxs-lookup"><span data-stu-id="0f217-194">To send the email, the code constructs the HTTP request, attaches the access token as an authorization header, and then posts the request to the send email endpoint.</span></span>

<span data-ttu-id="0f217-195">最後に、コードは電子メールが成功したかどうかをユーザーに通知するために返される HTTP 応答コードを使用します。</span><span class="sxs-lookup"><span data-stu-id="0f217-195">Finally, the code uses the HTTP response code returned to notify the user whether or not the email was successful.</span></span>

## <a name="run-the-app"></a><span data-ttu-id="0f217-196">アプリの実行</span><span class="sxs-lookup"><span data-stu-id="0f217-196">Run the app</span></span>

1. <span data-ttu-id="0f217-197">次のコマンドを使って、Rails アプリケーションと依存関係をインストールします。</span><span class="sxs-lookup"><span data-stu-id="0f217-197">Install the Rails application and dependencies with the following command.</span></span>

    ```
    bundle install
    ```
2. <span data-ttu-id="0f217-198">Rails アプリケーションを起動するには、次のコマンドを入力します。</span><span class="sxs-lookup"><span data-stu-id="0f217-198">To start the Rails application, type the following command.</span></span>

    ```
    rackup -p 3000
    ```
3. <span data-ttu-id="0f217-199">Web ブラウザーで `http://localhost:3000` にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="0f217-199">Go to `http://localhost:3000` in your web browser.</span></span>

## <a name="see-also"></a><span data-ttu-id="0f217-200">関連項目</span><span class="sxs-lookup"><span data-stu-id="0f217-200">See also</span></span>
- <span data-ttu-id="0f217-201">[Graph エクスプローラー](https://graph.microsoft.io/graph-explorer)を使用して REST API を試してみます。</span><span class="sxs-lookup"><span data-stu-id="0f217-201">Try out the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>
- <span data-ttu-id="0f217-202">GitHub の他の [Microsoft Graph サンプル](https://github.com/microsoftgraph)を探索します。</span><span class="sxs-lookup"><span data-stu-id="0f217-202">Explore our other [Microsoft Graph samples](https://github.com/microsoftgraph) on GitHub.</span></span>


