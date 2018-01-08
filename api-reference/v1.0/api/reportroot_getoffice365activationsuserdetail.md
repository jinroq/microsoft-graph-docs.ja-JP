# <a name="reportroot-getoffice365activationsuserdetail"></a><span data-ttu-id="57d1c-101">reportRoot: getOffice365ActivationsUserDetail</span><span class="sxs-lookup"><span data-stu-id="57d1c-101">reportRoot: getOffice365ActivationsUserDetail</span></span>

<span data-ttu-id="57d1c-102">Office 365 がアクティブ化されているユーザーに関する詳細情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="57d1c-102">Get details about users who have activated Office 365.</span></span>

> <span data-ttu-id="57d1c-103">**注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: Microsoft Office ライセンス認証]((https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60))」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="57d1c-103">**Note:** For details about different report views and names, see [Office 365 Reports - Microsoft Office activations]((https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)).</span></span>

## <a name="permissions"></a><span data-ttu-id="57d1c-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="57d1c-104">Permissions</span></span>

<span data-ttu-id="57d1c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="57d1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="57d1c-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="57d1c-107">Permission type</span></span>                        | <span data-ttu-id="57d1c-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="57d1c-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="57d1c-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="57d1c-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="57d1c-110">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57d1c-110">Not supported.</span></span>                           |
| <span data-ttu-id="57d1c-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="57d1c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57d1c-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57d1c-112">Not supported.</span></span>                           |
| <span data-ttu-id="57d1c-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="57d1c-113">Application</span></span>                            | <span data-ttu-id="57d1c-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="57d1c-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="57d1c-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="57d1c-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActivationsUserDetail
```

## <a name="request-headers"></a><span data-ttu-id="57d1c-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="57d1c-116">Request headers</span></span>

| <span data-ttu-id="57d1c-117">名前</span><span class="sxs-lookup"><span data-stu-id="57d1c-117">Name</span></span>          | <span data-ttu-id="57d1c-118">説明</span><span class="sxs-lookup"><span data-stu-id="57d1c-118">Description</span></span>                              |
| :------------ | :--------------------------------------- |
| <span data-ttu-id="57d1c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="57d1c-119">Authorization</span></span> | <span data-ttu-id="57d1c-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="57d1c-p102">Bearer {token}. Required.</span></span>                |
| <span data-ttu-id="57d1c-122">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="57d1c-122">if-none-match</span></span> | <span data-ttu-id="57d1c-123">この要求ヘッダーが含まれている場合、指定された eTag がファイルの現在のタグに一致すると、`304 Not Modified` 応答コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="57d1c-123">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `304 Not Modified` response is returned.</span></span> <span data-ttu-id="57d1c-124">省略可能。</span><span class="sxs-lookup"><span data-stu-id="57d1c-124">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="57d1c-125">応答</span><span class="sxs-lookup"><span data-stu-id="57d1c-125">Response</span></span>

<span data-ttu-id="57d1c-126">成功すると、レポートの事前認証されたダウンロード URL にリダイレクトする `302 Found` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="57d1c-126">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="57d1c-127">その URL は、応答の `Location` ヘッダー内にあります。</span><span class="sxs-lookup"><span data-stu-id="57d1c-127">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="57d1c-128">事前認証されたダウンロード URL は、短期間 (数分) のみ有効で、`Authorization` ヘッダーを必要としません。</span><span class="sxs-lookup"><span data-stu-id="57d1c-128">Pre-authenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header to download.</span></span>

<span data-ttu-id="57d1c-129">この CSV ファイルには、次の列ヘッダーがあります。</span><span class="sxs-lookup"><span data-stu-id="57d1c-129">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="57d1c-130">レポートの更新日</span><span class="sxs-lookup"><span data-stu-id="57d1c-130">Report Refresh Date</span></span>
- <span data-ttu-id="57d1c-131">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="57d1c-131">User Principal Name</span></span>
- <span data-ttu-id="57d1c-132">表示名</span><span class="sxs-lookup"><span data-stu-id="57d1c-132">Display Name</span></span>
- <span data-ttu-id="57d1c-133">製品の種類</span><span class="sxs-lookup"><span data-stu-id="57d1c-133">Product External Content Type</span></span>
- <span data-ttu-id="57d1c-134">最後のライセンス認証日</span><span class="sxs-lookup"><span data-stu-id="57d1c-134">Last Activated Date</span></span>
- <span data-ttu-id="57d1c-135">Windows</span><span class="sxs-lookup"><span data-stu-id="57d1c-135">Windows</span></span>
- <span data-ttu-id="57d1c-136">Mac</span><span class="sxs-lookup"><span data-stu-id="57d1c-136">Mac</span></span>
- <span data-ttu-id="57d1c-137">Windows 10 Mobile</span><span class="sxs-lookup"><span data-stu-id="57d1c-137">Windows 10 Mobile</span></span>
- <span data-ttu-id="57d1c-138">iOS</span><span class="sxs-lookup"><span data-stu-id="57d1c-138">iOS</span></span>
- <span data-ttu-id="57d1c-139">Android</span><span class="sxs-lookup"><span data-stu-id="57d1c-139">Android</span></span>

## <a name="example"></a><span data-ttu-id="57d1c-140">例</span><span class="sxs-lookup"><span data-stu-id="57d1c-140">Example</span></span>

#### <a name="request"></a><span data-ttu-id="57d1c-141">要求</span><span class="sxs-lookup"><span data-stu-id="57d1c-141">Request</span></span>

<span data-ttu-id="57d1c-142">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="57d1c-142">The following is an example of the request body.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activationsuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getOffice365ActivationsUserDetail
```

#### <a name="response"></a><span data-ttu-id="57d1c-143">応答</span><span class="sxs-lookup"><span data-stu-id="57d1c-143">Response</span></span>

<span data-ttu-id="57d1c-144">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="57d1c-144">The following is an example of a response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="57d1c-145">302 リダイレクトに従うと、ダウンロードされる CSV ファイルは次のスキーマを持つことになります。</span><span class="sxs-lookup"><span data-stu-id="57d1c-145">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Product Type,Last Activated Date,Windows,Mac,Windows 10 Mobile,iOS,Android
```
