# <a name="list-deleted-items-owned-by-a-user"></a><span data-ttu-id="37c1a-101">**ユーザーによって所有されている削除済みのアイテムを一覧表示します。**</span><span class="sxs-lookup"><span data-stu-id="37c1a-101">**List deleted items owned by a user**</span></span>

<span data-ttu-id="37c1a-102">指定されたユーザーによって所有されている、最近削除したアイテムの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="37c1a-102">Retrieves a list of recently deleted items owned by the specified user.</span></span>  

<span data-ttu-id="37c1a-103">現在、削除されたリスト アイテムの機能はユーザーによって所有されているリソースを[グループ化](../resources/group.md)します。</span><span class="sxs-lookup"><span data-stu-id="37c1a-103">Currently, list deleted items functionality is supported only for [group](../resources/group.md) resources owned by the user.</span></span>

<span data-ttu-id="37c1a-104">これは、改ページ調整がサポートされていないこと、サービスの操作です。</span><span class="sxs-lookup"><span data-stu-id="37c1a-104">This is a service action, which means it does not support pagination.</span></span>  <span data-ttu-id="37c1a-105">API が ID で並べ替えて、ユーザーが所有する最大 1,000 の削除されたオブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="37c1a-105">The API returns up to 1,000 deleted objects owned by the user, sorted by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="37c1a-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="37c1a-106">Permissions</span></span>

<span data-ttu-id="37c1a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="37c1a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

| <span data-ttu-id="37c1a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="37c1a-109">Permission type</span></span> | <span data-ttu-id="37c1a-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="37c1a-110">Permissions (from least to most privileged)</span></span> |
| --- | --- |
| <span data-ttu-id="37c1a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="37c1a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="37c1a-112">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37c1a-112">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="37c1a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="37c1a-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="37c1a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37c1a-114">Not supported.</span></span> |
| <span data-ttu-id="37c1a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="37c1a-115">Application</span></span> | <span data-ttu-id="37c1a-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37c1a-116">Group.Read.All, Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="37c1a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="37c1a-117">HTTP request</span></span>

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a><span data-ttu-id="37c1a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37c1a-118">Request headers</span></span>

| <span data-ttu-id="37c1a-119">名前</span><span class="sxs-lookup"><span data-stu-id="37c1a-119">Name</span></span>          | <span data-ttu-id="37c1a-120">説明</span><span class="sxs-lookup"><span data-stu-id="37c1a-120">Description</span></span>               |
| ------------- | ------------------------- |
| <span data-ttu-id="37c1a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="37c1a-121">Authorization</span></span> | <span data-ttu-id="37c1a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="37c1a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37c1a-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="37c1a-124">Request body</span></span>

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

<span data-ttu-id="37c1a-125">要求の本体には、次のパラメーターが必要です。</span><span class="sxs-lookup"><span data-stu-id="37c1a-125">The request body requires the following parameters:</span></span>

| <span data-ttu-id="37c1a-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="37c1a-126">Parameter</span></span>    | <span data-ttu-id="37c1a-127">型</span><span class="sxs-lookup"><span data-stu-id="37c1a-127">Type</span></span> |<span data-ttu-id="37c1a-128">説明</span><span class="sxs-lookup"><span data-stu-id="37c1a-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37c1a-129">userId</span><span class="sxs-lookup"><span data-stu-id="37c1a-129">userId</span></span>|<span data-ttu-id="37c1a-130">String</span><span class="sxs-lookup"><span data-stu-id="37c1a-130">String</span></span>|<span data-ttu-id="37c1a-131">所有者の ID です。</span><span class="sxs-lookup"><span data-stu-id="37c1a-131">ID of the owner.</span></span>|
|<span data-ttu-id="37c1a-132">type</span><span class="sxs-lookup"><span data-stu-id="37c1a-132">type</span></span>|<span data-ttu-id="37c1a-133">文字列</span><span class="sxs-lookup"><span data-stu-id="37c1a-133">String</span></span>|<span data-ttu-id="37c1a-134">返される所有しているオブジェクトの種類`Group`は、現在サポートされている値だけです。</span><span class="sxs-lookup"><span data-stu-id="37c1a-134">Type of owned objects to return; `Group` is currently the only supported value.</span></span>|


## <a name="response"></a><span data-ttu-id="37c1a-135">応答</span><span class="sxs-lookup"><span data-stu-id="37c1a-135">Response</span></span>

<span data-ttu-id="37c1a-136">成功した要求を返す`200 OK`応答コードです。応答オブジェクトには、[ディレクトリ (削除済みアイテム)](../resources/directory.md)のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="37c1a-136">Successful requests return `200 OK` response codes; the response object includes [directory (deleted items)](../resources/directory.md) properties.</span></span>

## <a name="example"></a><span data-ttu-id="37c1a-137">例</span><span class="sxs-lookup"><span data-stu-id="37c1a-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="37c1a-138">要求</span><span class="sxs-lookup"><span data-stu-id="37c1a-138">Request</span></span>

<span data-ttu-id="37c1a-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="37c1a-139">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a><span data-ttu-id="37c1a-140">応答</span><span class="sxs-lookup"><span data-stu-id="37c1a-140">Response</span></span>

<span data-ttu-id="37c1a-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="37c1a-141">Here is an example of the response.</span></span> <span data-ttu-id="37c1a-142">注: この応答オブジェクトを簡潔にするためにあります。</span><span class="sxs-lookup"><span data-stu-id="37c1a-142">Note: This response object may be truncated for brevity.</span></span> <span data-ttu-id="37c1a-143">サポートされているすべてのプロパティは、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="37c1a-143">All supported properties are returned from actual calls.</span></span>

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": 2018-04-01T12:39:16Z,
              "classification": null,
              "createdDateTime": "2017-03-22T12:39:16Z",
              "description": null,
              "displayName": "Test",
              "groupTypes": [
                  "Unified"
              ],
              "mail": "Test@contoso.com",
              "mailEnabled": true,
              "mailNickname": "Test",
              "membershipRule": null,
              "membershipRuleProcessingState": null,
              "preferredDataLocation": null,
              "preferredLanguage": null,
              "proxyAddresses": [
                  "SMTP:Test@contoso.com"
              ],
              "renewedDateTime": "2017-09-22T22:30:39Z",
              "securityEnabled": false,
              "theme": null,
              "visibility": "Public"
          } 
        ]
 }
```


