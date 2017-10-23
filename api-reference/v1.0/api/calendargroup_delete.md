# <a name="delete-calendargroup"></a><span data-ttu-id="04518-101">Delete calendarGroup</span><span class="sxs-lookup"><span data-stu-id="04518-101">Delete calendarGroup</span></span>

<span data-ttu-id="04518-102">既定の予定表グループ以外の予定表グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="04518-102">Delete a calendar group other than the default calendar group.</span></span>

<span data-ttu-id="04518-p101">**注**： Outlook.com によってサポートされるのは、/me/calendars ショートカットでアクセス可能な既定の予定表グループのみです。Outlook.com で他の予定表グループを削除することはできません。</span><span class="sxs-lookup"><span data-stu-id="04518-p101">**Note** Outlook.com supports only the default calendar group which is accessible by the /me/calendars shortcut. You cannot delete any calendar group in Outlook.com.</span></span>

## <a name="permissions"></a><span data-ttu-id="04518-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="04518-105">Permissions</span></span>
<span data-ttu-id="04518-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04518-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="04518-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04518-108">Permission type</span></span>      | <span data-ttu-id="04518-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="04518-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04518-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04518-110">Delegated (work or school account)</span></span> | <span data-ttu-id="04518-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04518-111">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="04518-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04518-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04518-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04518-113">Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="04518-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04518-114">Application</span></span> | <span data-ttu-id="04518-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04518-115">Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="04518-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04518-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="04518-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04518-117">Request headers</span></span>
| <span data-ttu-id="04518-118">名前</span><span class="sxs-lookup"><span data-stu-id="04518-118">Name</span></span>       | <span data-ttu-id="04518-119">型</span><span class="sxs-lookup"><span data-stu-id="04518-119">Type</span></span> | <span data-ttu-id="04518-120">説明</span><span class="sxs-lookup"><span data-stu-id="04518-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="04518-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="04518-121">Authorization</span></span>  | <span data-ttu-id="04518-122">string</span><span class="sxs-lookup"><span data-stu-id="04518-122">string</span></span>  | <span data-ttu-id="04518-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="04518-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04518-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="04518-125">Request body</span></span>
<span data-ttu-id="04518-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="04518-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04518-127">応答</span><span class="sxs-lookup"><span data-stu-id="04518-127">Response</span></span>

<span data-ttu-id="04518-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="04518-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04518-130">例</span><span class="sxs-lookup"><span data-stu-id="04518-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04518-131">要求</span><span class="sxs-lookup"><span data-stu-id="04518-131">Request</span></span>
<span data-ttu-id="04518-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="04518-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```
##### <a name="response"></a><span data-ttu-id="04518-133">応答</span><span class="sxs-lookup"><span data-stu-id="04518-133">Response</span></span>
<span data-ttu-id="04518-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="04518-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
