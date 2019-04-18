---
title: Microsoft Graph で Excel ブックにデータを書き込む
description: q = excelstarter)。
localization_priority: Priority
author: lumine2008
ms.prod: excel
ms.openlocfilehash: a8fcc90d4050cb6f0db2fb5e2b3a22d267f8cede
ms.sourcegitcommit: bbe42a15dad4ffe037a6934ab6001b585b7574c2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/17/2019
ms.locfileid: "31904071"
---
# <a name="write-data-to-an-excel-workbook-with-microsoft-graph"></a>Microsoft Graph で Excel ブックにデータを書き込む

Excel REST API は、情報を Excel ブックにアップロードするための、プラットフォームに依存しない簡単な手段を提供します。 このトピックでは、ASP.NET、Angular、および React の 3 種類の Web 開発フレームワークで、シンプルなデータ セットを Excel ブックに書き込む方法を示します。 このトピックで示されているサンプル コードは、[GitHub 上の Microsoft Graph Excel スターター サンプル](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=excelstarter)で確認できます。

> **注:** 3 つのサンプルのいずれも、データを **demo.xlsx** という名前の Excel ブックに書き込みます。 このブックが提供されているのは、それを自分の OneDrive にアップロードできるからですが、Microsoft Graph を使用することによっても、ファイルを OneDrive にアップロードできます。 いずれかのタイプのファイルをルート OneDrive フォルダーにアップロードするための REST 呼び出しに関する詳細は、[Microsoft Graph Excel REST API ASP.NET の予定リスト サンプル](https://github.com/microsoftgraph/aspnet-todo-rest-sample)を参照してください。

3 つの Excel スターター サンプルのいずれも、実行内容は同じです: サインイン ユーザーの名前とアドレスを取得し、それら 2 つの情報を **demo.xlsx** ブックの新しい行に追加します。 サンプルに変更を加えることにより、追加する行を表す 2 次元配列に情報を追加するという方法で、シンプルな操作で行を追加することができます。

## <a name="add-a-row-or-rows-to-an-excel-workbook-with-a-single-rest-request"></a>単一の REST 要求により Excel ブックに 1 行または複数行を追加する

Excel REST API では、シンプルな要求本体を、Excel ブックの行コレクションを表す REST エンドポイントに POST する必要があります。 サインイン ユーザーの OneDrive アカウントのルート フォルダーでノートブックを処理する場合、REST エンドポイントは次のようになります:

`https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add`

OneDrive フォルダー内のファイルにアクセスする方法については、リファレンス ドキュメントの中の「[DriveItem リソース タイプ](/graph/api/resources/driveitem?view=graph-rest-1.0)」を参照してください。

> **注:** ブックの既存の行コレクションを確認するには、パスのうち末尾が `/rows` の部分に対して、GET 要求を発行します。

POST 本体は次のようになります:

`{
  "index": null,
  "values": [
    ['alex darrow', 'adarrow@tenant.onmicrosoft.com']
  ]
}`

最初の `index` パラメーターの値は、行配列のうち、行を追加する相対位置を、0 から始まるインデックスにより指定します。 挿入した行より下の行が下方向にシフトします。 `null` パラメーターは、新しい行を末尾に追加することを示します。

第 2 の`values` パラメーターの値は、追加する各行の書式未設定の値を内容とする 2 次元文字列配列です。 サンプルの配列に含まれるのは 1 行だけですが、文字列配列をさらに追加することにより、さらに多くの行を追加できます。

demo.xlsx ファイルを OneDrive ルート フォルダーにアップロードし、[Microsoft Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) に対してこのクエリを実行することにより、自分の OneDrive アカウントでこのクエリをテストできます。

Excel ブックにデータを書き込むために必要なことは、これですべてです。 あとは、自分の使用するフレームワークで要求を作成して発行する方法を知る必要があります。Excel スターター サンプルで、3 種類の方法でこれを実行する方法が示されています。

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-aspnet"></a>Excel ブックに 1 行または複数行を追加する (ASP.NET)

要求を作成して送信する ASP.NET コードは、[Microsoft Graph Excel スターター サンプル (ASP.NET 4.6)](https://github.com/microsoftgraph/aspnet-excelstarter-sample) の [GraphResources.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphResources.cs) および [GraphService.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphService.cs) のファイルにあります。

`GraphResources.cs` ファイルは、Microsoft Graph から取り出すユーザー データと、ブックに書き込む際に使用する要求本体の両方をカプセル化するためのヘルパー クラスを提供します。

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

`GraphService.cs` クラスには、それらのクラスのデータを設定し、要求の情報をシリアライズして JSON オブジェクトに格納し、そのオブジェクトを POST 要求本体として渡す `AddInfoToExcel` メソッドが含まれています。

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

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-angular"></a>Excel ブックに 1 行または複数行を追加する (Angular)

要求を作成して送信する Angular コードは、[Microsoft Graph Excel スターター サンプル (Angular)](https://github.com/microsoftgraph/angular-excelstarter-sample) の [home.service.ts ファイル](https://github.com/microsoftgraph/angular-excelstarter-sample/blob/master/src/app/home/home.service.ts)に含まれています。

このサンプルでは TypeScript が使用されているため、これは、[Microsoft Graph JavaScript クライアント ライブラリ](https://github.com/microsoftgraph/msgraph-sdk-javascript)および [Microsoft Graph TypeScript のタイプ](https://github.com/microsoftgraph/msgraph-typescript-typings)を利用しています。

`home.service.ts` ファイルに含まれている `addInfoToExcel` 関数は、2 次元文字列配列、およびその配列が含まれる要求本体を作成します。 その後、Microsoft Graph JavaScript クライアント ライブラリを使用して要求を作成し、送信します。 応答は、Promise の形で返されます。

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

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-react"></a>Excel ブックに 1 行または複数行を追加する (React)

要求を作成して送信するコードは、[Microsoft Graph Excel スターター サンプル (React)](https://github.com/microsoftgraph/react-excelstarter-sample) の [home.js ファイル](https://github.com/microsoftgraph/react-excelstarter-sample/blob/master/src/home/home.js)に含まれています。

`onWriteToExcel` 関数は、2 次元文字列配列を作成し、それを要求本体に渡します。 これは、[axios](https://www.npmjs.com/package/axios) を使用することにより、HTTP 要求を発行します。

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

##<a name="see-also"></a>関連項目

* [Microsoft Graph で Excel のセッションを管理する](excel-manage-sessions.md)
* [Microsoft Graph で Excel のブック関数を使用する](excel-use-functions.md)
* [Microsoft Graph により Excel のある範囲の書式を更新する](excel-update-range-format.md)
* [Microsoft Graph により Excel のグラフ イメージを表示する](excel-display-chart-image.md)
* [Excel REST API を使用する](/graph/api/resources/excel?view=graph-rest-1.0)    
