# <a name="write-data-to-an-excel-workbook-with-microsoft-graph"></a><span data-ttu-id="c7ca6-101">Microsoft Graph で Excel ブックにデータを書き込む</span><span class="sxs-lookup"><span data-stu-id="c7ca6-101">Write data to an Excel workbook with Microsoft Graph</span></span>

<span data-ttu-id="c7ca6-102">Excel REST API は、情報を Excel ブックにアップロードするための、プラットフォームに依存しない簡単な手段を提供します。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-102">The Excel REST API provides an easy, platform-agnostic way to upload information to an Excel workbook.</span></span> <span data-ttu-id="c7ca6-103">このトピックでは、ASP.NET、Angular、および React の 3 種類の Web 開発フレームワークで、シンプルなデータ セットを Excel ブックに書き込む方法を示します。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-103">This topic shows you how to write simple data sets to an Excel workbook on three web development frameworks: ASP.NET, Angular, and React.</span></span> <span data-ttu-id="c7ca6-104">このトピックで示されているサンプル コードは、[GitHub 上の Microsoft Graph Excel スターター サンプル](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=excelstarter)で確認できます。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-104">You can look at the code samples featured in this topic by visiting the [Microsoft Graph Excel starter samples on GitHub](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=excelstarter).</span></span>

> <span data-ttu-id="c7ca6-105">**注:** 3 つのサンプルのいずれも、データを **demo.xlxs** という名前の Excel ブックに書き込みます。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-105">**Note:** All three of the samples write data to an Excel workbook named **demo.xlxs**.</span></span> <span data-ttu-id="c7ca6-106">このブックが提供されているのは、それを自分の OneDrive にアップロードできるからですが、Microsoft Graph を使用することによっても、ファイルを OneDrive にアップロードできます。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-106">They provide this workbook for you so that you can upload it to your own OneDrive, but you can also use Microsoft Graph to upload files to OneDrive.</span></span> <span data-ttu-id="c7ca6-107">いずれかのタイプのファイルをルート OneDrive フォルダーにアップロードするための REST 呼び出しに関する詳細は、[Microsoft Graph Excel REST API ASP.NET の予定リスト サンプル](https://github.com/microsoftgraph/aspnet-todo-rest-sample)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-107">If you're interested in learning the REST calls you need to upload a file of any type to your root OneDrive folder, see the [Microsoft Graph Excel REST API ASP.NET to-do list sample](https://github.com/microsoftgraph/aspnet-todo-rest-sample).</span></span>

<span data-ttu-id="c7ca6-108">3 つの Excel スターター サンプルのいずれも、実行内容は同じです: サインイン ユーザーの名前とアドレスを取得し、それら 2 つの情報を **demo.xlsx** ブックの新しい行に追加します。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-108">All three of the Excel starter samples do the same thing: retrieve the name and address of the signed-in user and add those two pieces of information to a new row in the **demo.xlsx** workbook.</span></span> <span data-ttu-id="c7ca6-109">サンプルに変更を加えることにより、追加する行を表す 2 次元配列に情報を追加するという方法で、シンプルな操作で行を追加することができます。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-109">You can modify the samples to add additional rows simply by adding information to the two-dimensional array that represents the row or rows that you want to add.</span></span>

## <a name="add-a-row-or-rows-to-an-excel-workbook-with-a-single-rest-request"></a><span data-ttu-id="c7ca6-110">単一の REST 要求により Excel ブックに 1 行または複数行を追加する</span><span class="sxs-lookup"><span data-stu-id="c7ca6-110">Add a row or rows to an Excel workbook with a single REST request</span></span>

<span data-ttu-id="c7ca6-111">Excel REST API では、シンプルな要求本体を、Excel ブックの行コレクションを表す REST エンドポイントに POST する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-111">The Excel REST API requires you to POST a simple request body to the REST endpoint that represents the row collection of an Excel workbook.</span></span> <span data-ttu-id="c7ca6-112">サインイン ユーザーの OneDrive アカウントのルート フォルダーでノートブックを処理する場合、REST エンドポイントは次のようになります:</span><span class="sxs-lookup"><span data-stu-id="c7ca6-112">If you're working with a notebook in the root folder of the signed-in user's OneDrive account, the REST endpoint will look like this:</span></span>

`https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add`

<span data-ttu-id="c7ca6-113">OneDrive フォルダー内のファイルにアクセスする方法については、リファレンス ドキュメントの中の「[DriveItem リソース タイプ](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/driveitem)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-113">For more information about how to reach files in OneDrive folders, see the [DriveItem resource type](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/resources/driveitem) in our reference documentation.</span></span>

> <span data-ttu-id="c7ca6-114">**注:** ブックの既存の行コレクションを確認するには、パスのうち末尾が `/rows` の部分に対して、GET 要求を発行します。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-114">**Note:** You can look at the existing row collection of the workbook by making a GET request to the part of the path that ends at `/rows`.</span></span>

<span data-ttu-id="c7ca6-115">POST 本体は次のようになります:</span><span class="sxs-lookup"><span data-stu-id="c7ca6-115">The POST body looks like this:</span></span>

`{
  "index": null,
  "values": [
    ['alex darrow', 'adarrow@tenant.onmicrosoft.com']
  ]
}`

<span data-ttu-id="c7ca6-116">最初の `index` パラメーターの値は、行配列のうち、行を追加する相対位置を、0 から始まるインデックスにより指定します。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-116">The value of the first `index` parameter specifies the relative position of the row that you're adding to the zero-indexed array of rows.</span></span> <span data-ttu-id="c7ca6-117">挿入した行より下の行が下方向にシフトします。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-117">Rows below the inserted row will be shifted downwards.</span></span> <span data-ttu-id="c7ca6-118">`null` パラメーターは、新しい行を末尾に追加することを示します。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-118">The `null` parameter indicates that the new row will be added to the end.</span></span>

<span data-ttu-id="c7ca6-119">第 2 の`values` パラメーターの値は、追加する各行の書式未設定の値を内容とする 2 次元文字列配列です。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-119">The value of the second `values` parameter is a two-dimensional string array that contains the unformatted values of each row that you want to add.</span></span> <span data-ttu-id="c7ca6-120">サンプルの配列に含まれるのは 1 行だけですが、文字列配列をさらに追加することにより、さらに多くの行を追加できます。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-120">The array in the sample contains only one row, but you can add more rows by adding more string arrays.</span></span>

<span data-ttu-id="c7ca6-121">demo.xlsx ファイルを OneDrive ルート フォルダーにアップロードし、[Microsoft Graph Explorer](https://developer.microsoft.com/ja-JP/graph/graph-explorer) に対してこのクエリを実行することにより、自分の OneDrive アカウントでこのクエリをテストできます。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-121">You can test this query with your own OneDrive account by uploading the demo.xlsx file to your OneDrive root folder and executing this query on the [Microsoft Graph Explorer](https://developer.microsoft.com/ja-JP/graph/graph-explorer).</span></span>

<span data-ttu-id="c7ca6-122">Excel ブックにデータを書き込むために必要なことは、これですべてです。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-122">That is all you need to know in order to write data to an Excel workbook.</span></span> <span data-ttu-id="c7ca6-123">あとは、自分の使用するフレームワークで要求を作成して発行する方法を知る必要があります。Excel スターター サンプルで、3 種類の方法でこれを実行する方法が示されています。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-123">You do need to know how to construct and make the request in your own framework, and the Excel starter samples demonstrate three separate ways of doing this.</span></span>

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-aspnet"></a><span data-ttu-id="c7ca6-124">Excel ブックに 1 行または複数行を追加する (ASP.NET)</span><span class="sxs-lookup"><span data-stu-id="c7ca6-124">Add a row or rows to an Excel workbook in ASP.NET</span></span>

<span data-ttu-id="c7ca6-125">要求を作成して送信する ASP.NET コードは、[Microsoft Graph Excel スターター サンプル (ASP.NET 4.6)](https://github.com/microsoftgraph/aspnet-excelstarter-sample) の [GraphResources.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphResources.cs) および [GraphService.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphService.cs) のファイルにあります。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-125">You'll find the ASP.NET code that constructs and sends the request in the [GraphResources.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphResources.cs) and [GraphService.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphService.cs) files of the [Microsoft Graph Excel Starter Sample for ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-excelstarter-sample).</span></span>

<span data-ttu-id="c7ca6-126">`GraphResources.cs` ファイルは、Microsoft Graph から取り出すユーザー データと、ブックに書き込む際に使用する要求本体の両方をカプセル化するためのヘルパー クラスを提供します。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-126">The `GraphResources.cs` file provides a helper class for encapsulating both the user data you're retrieving from Microsoft Graph and the request body that you'll use when you write to your workbook.</span></span>

    public class UserInfo
    {
        public string Name { get; set; }
        public string Address { get; set; }

    }

    public class UserInfoRequest
    {
        public string index { get; set; }
        public string[][] values { get; set; }
    }

<span data-ttu-id="c7ca6-127">`GraphService.cs` クラスには、それらのクラスのデータを設定し、要求の情報をシリアライズして JSON オブジェクトに格納し、そのオブジェクトを POST 要求本体として渡す `AddInfoToExcel` メソッドが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-127">The `GraphService.cs` class contains an `AddInfoToExcel` method that populates these classes, serializes the request information into a JSON object, and then passes that object as the POST request body.</span></span>

        public async Task<string> AddInfoToExcel(string accessToken, string name, string address)
        {
            string endpoint = "https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add";
            using (var client = new HttpClient())
            {
                using (var request = new HttpRequestMessage(HttpMethod.Post, endpoint))
                {
                    // Populate UserInfoRequest object
                    string[] userInfo = { name, address  };
                    string[][] userInfoArray = { userInfo };
                    UserInfoRequest userInfoRequest = new UserInfoRequest();
                    userInfoRequest.index = null;
                    userInfoRequest.values = userInfoArray;

                    // Serialize the information in the UserInfoRequest object
                    string jsonBody = JsonConvert.SerializeObject(userInfoRequest);
                    request.Headers.Accept.Add(new MediaTypeWithQualityHeaderValue("application/json"));
                    request.Headers.Authorization = new AuthenticationHeaderValue("Bearer", accessToken);
                    request.Content = new StringContent(jsonBody, Encoding.UTF8, "application/json");

                    using (var response = await client.SendAsync(request))
                    {
                        if (response.IsSuccessStatusCode)
                        {
                            return Resource.Graph_UploadToExcel_Success_Result;
                        }
                        return response.ReasonPhrase;
                    }
                }
            }
        }

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-angular"></a><span data-ttu-id="c7ca6-128">Excel ブックに 1 行または複数行を追加する (Angular)</span><span class="sxs-lookup"><span data-stu-id="c7ca6-128">Add a row or rows to an Excel workbook in Angular</span></span>

<span data-ttu-id="c7ca6-129">要求を作成して送信する Angular コードは、[Microsoft Graph Excel スターター サンプル (Angular)](https://github.com/microsoftgraph/angular-excelstarter-sample) の [home.service.ts ファイル](https://github.com/microsoftgraph/angular-excelstarter-sample/blob/master/src/app/home/home.service.ts)に含まれています。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-129">You'll find the Angular code that constructs and sends the request in the [home.service.ts file](https://github.com/microsoftgraph/angular-excelstarter-sample/blob/master/src/app/home/home.service.ts) of the [Microsoft Graph Excel Starter Sample for Angular](https://github.com/microsoftgraph/angular-excelstarter-sample).</span></span>

<span data-ttu-id="c7ca6-130">このサンプルでは TypeScript が使用されているため、これは、[Microsoft Graph JavaScript クライアント ライブラリ](https://github.com/microsoftgraph/msgraph-sdk-javascript)および [Microsoft Graph TypeScript のタイプ](https://github.com/microsoftgraph/msgraph-typescript-typings)を利用しています。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-130">Since this sample uses TypeScript, it takes advantage of the [Microsoft Graph JavaScript Client Library](https://github.com/microsoftgraph/msgraph-sdk-javascript) and the [ Microsoft Graph TypeScript Types](https://github.com/microsoftgraph/msgraph-typescript-typings).</span></span>

<span data-ttu-id="c7ca6-131">`home.service.ts` ファイルに含まれている `addInfoToExcel` 関数は、2 次元文字列配列、およびその配列が含まれる要求本体を作成します。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-131">The `addInfoToExcel` function in the `home.service.ts` file constructs the two-dimensional string array and the request body that contains the array.</span></span> <span data-ttu-id="c7ca6-132">その後、Microsoft Graph JavaScript クライアント ライブラリを使用して要求を作成し、送信します。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-132">It then uses the Microsoft Graph JavaScript Client Library to construct and send the request.</span></span> <span data-ttu-id="c7ca6-133">応答は、Promise の形で返されます。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-133">The response comes back in the form of a Promise.</span></span>

      addInfoToExcel(user: MicrosoftGraph.User) {
        const userInfo = [];
        const userEmail = user.mail || user.userPrincipalName;    
        userInfo.push([user.displayName, userEmail]);

        const userInfoRequestBody = {
          index: null,
          values: userInfo
        };   

        const body = JSON.stringify(userInfoRequestBody);

        var client = this.getClient();
        var url = `${this.url}/me/drive/root:/${this.file}:/workbook/tables/${this.table}/rows/add`
        return Observable.fromPromise(client
        .api(url)
        .post(body)
        );
      }

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-react"></a><span data-ttu-id="c7ca6-134">Excel ブックに 1 行または複数行を追加する (React)</span><span class="sxs-lookup"><span data-stu-id="c7ca6-134">Add a row or rows to an Excel workbook in React</span></span>

<span data-ttu-id="c7ca6-135">要求を作成して送信するコードは、[Microsoft Graph Excel スターター サンプル (React)](https://github.com/microsoftgraph/react-excelstarter-sample) の [home.js ファイル](https://github.com/microsoftgraph/react-excelstarter-sample/blob/master/src/home/home.js)に含まれています。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-135">You'll find the code that constructs and sends the request in the [home.js file](https://github.com/microsoftgraph/react-excelstarter-sample/blob/master/src/home/home.js) of the [Microsoft Graph Excel Starter Sample for React](https://github.com/microsoftgraph/react-excelstarter-sample).</span></span>

<span data-ttu-id="c7ca6-136">`onWriteToExcel` 関数は、2 次元文字列配列を作成し、それを要求本体に渡します。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-136">The `onWriteToExcel` function constructs the two-dimensional string array and passes it as the request body.</span></span> <span data-ttu-id="c7ca6-137">これは、[axios](https://www.npmjs.com/package/axios) を使用することにより、HTTP 要求を発行します。</span><span class="sxs-lookup"><span data-stu-id="c7ca6-137">It uses [axios](https://www.npmjs.com/package/axios) to make the HTTP request.</span></span>

      onWriteToExcel() {
        const { token, me } = this.state;

        const myEmailAddress = me.mail || me.userPrincipalName;
        const values = [];

        values.push([me.displayName, myEmailAddress]);

        axios
          .post('https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add',
            { index: null, values },
            { headers: { Authorization: `Bearer ${token}` }}
          )
          .then(res => {
                          console.log(res);
                          const successMessage = "Successfully wrote your data to demo.xlsx!";
                          this.setState ({ successMessage });
                         })
          .catch(err => console.error(err));
      }

##<a name="see-also"></a><span data-ttu-id="c7ca6-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="c7ca6-138">See also</span></span>

* [<span data-ttu-id="c7ca6-139">Microsoft Graph で Excel のセッションを管理する</span><span class="sxs-lookup"><span data-stu-id="c7ca6-139">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="c7ca6-140">Microsoft Graph で Excel のブック関数を使用する</span><span class="sxs-lookup"><span data-stu-id="c7ca6-140">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="c7ca6-141">Microsoft Graph により Excel のある範囲の書式を更新する</span><span class="sxs-lookup"><span data-stu-id="c7ca6-141">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="c7ca6-142">Microsoft Graph により Excel のグラフ イメージを表示する</span><span class="sxs-lookup"><span data-stu-id="c7ca6-142">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="c7ca6-143">Excel REST API を使用する</span><span class="sxs-lookup"><span data-stu-id="c7ca6-143">Use the Outlook REST API</span></span>](../api-reference/v1.0/resources/excel.md)    
