# <a name="delete-open-extension"></a><span data-ttu-id="3d5f2-101">オープン拡張機能を削除する</span><span class="sxs-lookup"><span data-stu-id="3d5f2-101">Delete open extension</span></span>

<span data-ttu-id="3d5f2-102">指定されたリソースのインスタンスからオープン拡張機能 ([openTypeExtension](../resources/openTypeExtension.md) オブジェクト) を削除します。</span><span class="sxs-lookup"><span data-stu-id="3d5f2-102">Delete an open extension ([openTypeExtension](../resources/openTypeExtension.md) object) from the specified instance of a resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="3d5f2-103">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3d5f2-103">Permissions</span></span>

<span data-ttu-id="3d5f2-p101">この API を呼び出すには、拡張機能を削除するリソースに応じて、以下のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3d5f2-p101">One of the following permissions is required to call this API, depending on the resource you're deleting the extension from. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3d5f2-106">**サポートされているリソース**</span><span class="sxs-lookup"><span data-stu-id="3d5f2-106">**Supported resource**</span></span>|<span data-ttu-id="3d5f2-107">**アクセス許可**</span><span class="sxs-lookup"><span data-stu-id="3d5f2-107">**Permission**</span></span>|<span data-ttu-id="3d5f2-108">**サポートされているリソース**</span><span class="sxs-lookup"><span data-stu-id="3d5f2-108">**Supported resource**</span></span>|<span data-ttu-id="3d5f2-109">**アクセス許可**</span><span class="sxs-lookup"><span data-stu-id="3d5f2-109">**Permission**</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="3d5f2-110">デバイス</span><span class="sxs-lookup"><span data-stu-id="3d5f2-110">device</span></span>](../resources/device.md) | <span data-ttu-id="3d5f2-111">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d5f2-111">Device.ReadWrite.All</span></span> | [<span data-ttu-id="3d5f2-112">イベント</span><span class="sxs-lookup"><span data-stu-id="3d5f2-112">event</span></span>](../resources/event.md) | <span data-ttu-id="3d5f2-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d5f2-113">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="3d5f2-114">グループ</span><span class="sxs-lookup"><span data-stu-id="3d5f2-114">group</span></span>](../resources/group.md) | <span data-ttu-id="3d5f2-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d5f2-115">Group.ReadWrite.All</span></span> | [<span data-ttu-id="3d5f2-116">グループ イベント</span><span class="sxs-lookup"><span data-stu-id="3d5f2-116">group event</span></span>](../resources/event.md) | <span data-ttu-id="3d5f2-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d5f2-117">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="3d5f2-118">グループの投稿</span><span class="sxs-lookup"><span data-stu-id="3d5f2-118">group post</span></span>](../resources/post.md) | <span data-ttu-id="3d5f2-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d5f2-119">Group.ReadWrite.All</span></span> | [<span data-ttu-id="3d5f2-120">メッセージ</span><span class="sxs-lookup"><span data-stu-id="3d5f2-120">message</span></span>](../resources/message.md) | <span data-ttu-id="3d5f2-121">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d5f2-121">Mail.ReadWrite</span></span> |
| [<span data-ttu-id="3d5f2-122">組織</span><span class="sxs-lookup"><span data-stu-id="3d5f2-122">organization</span></span>](../resources/organization.md) | <span data-ttu-id="3d5f2-123">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3d5f2-123">Directory.AccessAsUser.All</span></span> | [<span data-ttu-id="3d5f2-124">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="3d5f2-124">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="3d5f2-125">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3d5f2-125">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="3d5f2-126">ユーザー</span><span class="sxs-lookup"><span data-stu-id="3d5f2-126">user</span></span>](../resources/user.md) | <span data-ttu-id="3d5f2-127">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3d5f2-127">Directory.AccessAsUser.All</span></span> | | |

## <a name="http-request"></a><span data-ttu-id="3d5f2-128">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3d5f2-128">HTTP request</span></span>
<span data-ttu-id="3d5f2-129">要求で、リソース インスタンスを識別し、そのインスタンスの **extensions** ナビゲーション プロパティを使用して拡張機能を識別し、その拡張インスタンスで `DELETE` を行います。</span><span class="sxs-lookup"><span data-stu-id="3d5f2-129">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `DELETE` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/extensions/{extensionId}
DELETE /groups/{id}/events/{id}/extensions/{extensionId}
DELETE /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
DELETE /organization/{Id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
DELETE /users/{id|userPrincipalName}/extensions/{extensionId}
```

><span data-ttu-id="3d5f2-p102">**注:**上記の構文は、拡張機能の削除元となるリソース インスタンスを特定する一般的な方法を示しています。こうしたリソース インスタンスを特定するために使用できる他の構文すべても、同様の方法でオープン拡張機能を削除できます。</span><span class="sxs-lookup"><span data-stu-id="3d5f2-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to delete an extension from it. All other syntax that allows you to identify these resource instances supports deleting open extensions from them in a similar way.</span></span>

## <a name="parameters"></a><span data-ttu-id="3d5f2-132">パラメーター</span><span class="sxs-lookup"><span data-stu-id="3d5f2-132">Parameters</span></span>
|<span data-ttu-id="3d5f2-133">**パラメーター**</span><span class="sxs-lookup"><span data-stu-id="3d5f2-133">**Parameter**</span></span>|<span data-ttu-id="3d5f2-134">**型**</span><span class="sxs-lookup"><span data-stu-id="3d5f2-134">**Type**</span></span>|<span data-ttu-id="3d5f2-135">**説明**</span><span class="sxs-lookup"><span data-stu-id="3d5f2-135">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3d5f2-136">_URL parameters_</span><span class="sxs-lookup"><span data-stu-id="3d5f2-136">_URL parameters_</span></span>|
|<span data-ttu-id="3d5f2-137">id</span><span class="sxs-lookup"><span data-stu-id="3d5f2-137">id</span></span>|<span data-ttu-id="3d5f2-138">string</span><span class="sxs-lookup"><span data-stu-id="3d5f2-138">string</span></span>|<span data-ttu-id="3d5f2-p103">対応するコレクションのインスタンスの一意識別子。必須。</span><span class="sxs-lookup"><span data-stu-id="3d5f2-p103">A unique identifier for an instance in the corresponding collection. Required.</span></span>|
|<span data-ttu-id="3d5f2-141">extensionId</span><span class="sxs-lookup"><span data-stu-id="3d5f2-141">extensionId</span></span>|<span data-ttu-id="3d5f2-142">string</span><span class="sxs-lookup"><span data-stu-id="3d5f2-142">string</span></span>|<span data-ttu-id="3d5f2-p104">これは、拡張情報の一意のテキスト識別子である拡張情報名、または拡張情報の種類と一意のテキスト識別子を連結した完全修飾名になります。完全修飾名は、拡張情報を作成したときに、`id` プロパティで返されます。必須。</span><span class="sxs-lookup"><span data-stu-id="3d5f2-p104">This can be an extension name which is a unique text identifier for the extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="3d5f2-146">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3d5f2-146">Request headers</span></span>
| <span data-ttu-id="3d5f2-147">名前</span><span class="sxs-lookup"><span data-stu-id="3d5f2-147">Name</span></span>       | <span data-ttu-id="3d5f2-148">値</span><span class="sxs-lookup"><span data-stu-id="3d5f2-148">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="3d5f2-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d5f2-149">Authorization</span></span> | <span data-ttu-id="3d5f2-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3d5f2-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d5f2-152">要求本文</span><span class="sxs-lookup"><span data-stu-id="3d5f2-152">Request body</span></span>
<span data-ttu-id="3d5f2-153">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3d5f2-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d5f2-154">応答</span><span class="sxs-lookup"><span data-stu-id="3d5f2-154">Response</span></span>

<span data-ttu-id="3d5f2-p106">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="3d5f2-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d5f2-157">例</span><span class="sxs-lookup"><span data-stu-id="3d5f2-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3d5f2-158">要求</span><span class="sxs-lookup"><span data-stu-id="3d5f2-158">Request</span></span>
<span data-ttu-id="3d5f2-159">最初の例では、名前で拡張情報を参照し、指定されたメッセージの拡張情報を削除します。</span><span class="sxs-lookup"><span data-stu-id="3d5f2-159">The first example references an extension by its name and deletes the extension in the specified message.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_opentypeextension"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions('Com.Contoso.Referral')
```

<span data-ttu-id="3d5f2-160">2 番目の例では、指定されたグループ イベントの拡張機能を削除します。</span><span class="sxs-lookup"><span data-stu-id="3d5f2-160">The second example deletes an extension in the specified group event.</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/groups('f5480dfd-7d77-4d0b-ba2e-3391953cc74a')/events('AAMkADVlN17IsAAA=')/extensions('Com.Contoso.Referral')
```

 

##### <a name="response"></a><span data-ttu-id="3d5f2-161">応答</span><span class="sxs-lookup"><span data-stu-id="3d5f2-161">Response</span></span>
<span data-ttu-id="3d5f2-162">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3d5f2-162">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->