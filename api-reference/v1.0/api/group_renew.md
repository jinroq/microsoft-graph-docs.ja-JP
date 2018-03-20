# <a name="group-renew"></a><span data-ttu-id="d7c93-101">group: renew</span><span class="sxs-lookup"><span data-stu-id="d7c93-101">group: renew</span></span>

<span data-ttu-id="d7c93-102">グループの有効期限を更新します。</span><span class="sxs-lookup"><span data-stu-id="d7c93-102">Renews a group's expiration.</span></span> <span data-ttu-id="d7c93-103">グループが更新されると、グループの有効期限はポリシーで定義された日数、延長されます。</span><span class="sxs-lookup"><span data-stu-id="d7c93-103">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7c93-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d7c93-104">Permissions</span></span>

<span data-ttu-id="d7c93-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7c93-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 

|<span data-ttu-id="d7c93-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d7c93-107">Permission type</span></span>      | <span data-ttu-id="d7c93-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d7c93-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7c93-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d7c93-109">Delegated (work or school account)</span></span> | <span data-ttu-id="d7c93-110">Group.ReadWrite.All または Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7c93-110">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="d7c93-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d7c93-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7c93-112">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="d7c93-112">Not supported</span></span> |
|<span data-ttu-id="d7c93-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d7c93-113">Application</span></span> | <span data-ttu-id="d7c93-114">Group.ReadWrite.All または Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7c93-114">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7c93-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d7c93-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/<id>/renew
```

## <a name="request-headers"></a><span data-ttu-id="d7c93-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d7c93-116">Request headers</span></span>
| <span data-ttu-id="d7c93-117">名前</span><span class="sxs-lookup"><span data-stu-id="d7c93-117">Name</span></span>       | <span data-ttu-id="d7c93-118">説明</span><span class="sxs-lookup"><span data-stu-id="d7c93-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d7c93-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7c93-119">Authorization</span></span>  | <span data-ttu-id="d7c93-120">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="d7c93-120">Bearer %token%</span></span> |


## <a name="request-body"></a><span data-ttu-id="d7c93-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="d7c93-121">Request body</span></span>

<span data-ttu-id="d7c93-122">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d7c93-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7c93-123">応答</span><span class="sxs-lookup"><span data-stu-id="d7c93-123">Response</span></span>

<span data-ttu-id="d7c93-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d7c93-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7c93-126">例</span><span class="sxs-lookup"><span data-stu-id="d7c93-126">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d7c93-127">要求</span><span class="sxs-lookup"><span data-stu-id="d7c93-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/<id>/renew
```

##### <a name="response"></a><span data-ttu-id="d7c93-128">応答</span><span class="sxs-lookup"><span data-stu-id="d7c93-128">Response</span></span>
<span data-ttu-id="d7c93-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d7c93-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Boolean"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: renew",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->