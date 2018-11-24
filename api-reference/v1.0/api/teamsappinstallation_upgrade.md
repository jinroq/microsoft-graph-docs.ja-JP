# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="398db-101">チームでアプリケーションをアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="398db-101">Upgrade an app in a team</span></span>



<span data-ttu-id="398db-102">[チーム](../resources/team.md)で[アプリケーションのインストール](../resources/teamsappinstallation.md)をアプリケーションの最新バージョンにアップグレードします。</span><span class="sxs-lookup"><span data-stu-id="398db-102">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="398db-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="398db-103">Permissions</span></span>

<span data-ttu-id="398db-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="398db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="398db-106">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="398db-106">Permission type</span></span>      | <span data-ttu-id="398db-107">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="398db-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="398db-108">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="398db-108">Delegated (work or school account)</span></span> | <span data-ttu-id="398db-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="398db-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="398db-110">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="398db-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="398db-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="398db-111">Not supported.</span></span>    |
|<span data-ttu-id="398db-112">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="398db-112">Application</span></span> | <span data-ttu-id="398db-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="398db-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="398db-114">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="398db-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="398db-115">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="398db-115">Request headers</span></span>
| <span data-ttu-id="398db-116">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="398db-116">Header</span></span>       | <span data-ttu-id="398db-117">値</span><span class="sxs-lookup"><span data-stu-id="398db-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="398db-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="398db-118">Authorization</span></span>  | <span data-ttu-id="398db-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="398db-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="398db-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="398db-121">Request body</span></span>
<span data-ttu-id="398db-122">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="398db-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="398db-123">応答</span><span class="sxs-lookup"><span data-stu-id="398db-123">Response</span></span>

<span data-ttu-id="398db-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="398db-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="398db-126">例</span><span class="sxs-lookup"><span data-stu-id="398db-126">Example</span></span>

#### <a name="request"></a><span data-ttu-id="398db-127">要求</span><span class="sxs-lookup"><span data-stu-id="398db-127">Request</span></span>
<span data-ttu-id="398db-128">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="398db-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
#### <a name="response"></a><span data-ttu-id="398db-129">応答</span><span class="sxs-lookup"><span data-stu-id="398db-129">Response</span></span>
<span data-ttu-id="398db-130">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="398db-130">The following is an example of the response.</span></span> 

><span data-ttu-id="398db-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="398db-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
