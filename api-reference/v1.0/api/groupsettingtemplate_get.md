# <a name="get-a-group-setting-template"></a><span data-ttu-id="73b7d-101">グループ設定テンプレートを取得する</span><span class="sxs-lookup"><span data-stu-id="73b7d-101">Get a group setting template</span></span>

<span data-ttu-id="73b7d-p101">グループ設定テンプレートは、テナント内で作成できる設定に基づいた設定のテンプレートを表します。この操作により、利用可能な設定とその既定値を含む、[groupSettingTemplate](../resources/groupsettingtemplate.md) オブジェクトのプロパティを取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="73b7d-p101">A group setting template represents a template of settings from which settings may be created within a tenant. This operation allows retrieval of the properties of the [groupSettingTemplate](../resources/groupsettingtemplate.md) object, including the available settings and their defaults.</span></span>

## <a name="permissions"></a><span data-ttu-id="73b7d-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="73b7d-104">Permissions</span></span>

<span data-ttu-id="73b7d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73b7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="73b7d-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="73b7d-107">Permission type</span></span>      | <span data-ttu-id="73b7d-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="73b7d-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73b7d-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="73b7d-109">Delegated (work or school account)</span></span> | <span data-ttu-id="73b7d-110">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="73b7d-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="73b7d-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="73b7d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73b7d-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73b7d-112">Not supported.</span></span>    |
|<span data-ttu-id="73b7d-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="73b7d-113">Application</span></span> | <span data-ttu-id="73b7d-114">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73b7d-114">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73b7d-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="73b7d-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="73b7d-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="73b7d-116">Optional query parameters</span></span>
<span data-ttu-id="73b7d-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="73b7d-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73b7d-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73b7d-118">Request headers</span></span>
| <span data-ttu-id="73b7d-119">名前</span><span class="sxs-lookup"><span data-stu-id="73b7d-119">Name</span></span> | <span data-ttu-id="73b7d-120">説明</span><span class="sxs-lookup"><span data-stu-id="73b7d-120">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="73b7d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="73b7d-121">Authorization</span></span> | <span data-ttu-id="73b7d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="73b7d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73b7d-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="73b7d-124">Request body</span></span>
<span data-ttu-id="73b7d-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="73b7d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73b7d-126">応答</span><span class="sxs-lookup"><span data-stu-id="73b7d-126">Response</span></span>

<span data-ttu-id="73b7d-127">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [groupSettingTemplate](../resources/groupsettingtemplate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="73b7d-127">If successful, this method returns a `200 OK` response code and [groupSettingTemplate](../resources/groupsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73b7d-128">例</span><span class="sxs-lookup"><span data-stu-id="73b7d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73b7d-129">要求</span><span class="sxs-lookup"><span data-stu-id="73b7d-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplate"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="73b7d-130">応答</span><span class="sxs-lookup"><span data-stu-id="73b7d-130">Response</span></span>

<span data-ttu-id="73b7d-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="73b7d-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1341

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates/$entity",
    "id": "62375ab9-6b52-47ed-826b-58e47e0e304b",
    "deletedDateTime": null,
    "displayName": "Group.Unified",
    "description": "Setting templates define the different settings that can be used for the associated ObjectSettings. This template defines settings that can be used for Unified Groups.",
    "values": [
        {
            "name": "CustomBlockedWordsList",
            "type": "System.String",
            "defaultValue": "",
            "description": "A comma-delimited list of blocked words for Unified Group displayName and mailNickName."
        },
        {
            "name": "EnableMSStandardBlockedWords",
            "type": "System.Boolean",
            "defaultValue": "false",
            "description": "A flag indicating whether or not to enable the Microsoft Standard list of blocked words for Unified Group displayName and mailNickName."
        },
        {
            "name": "ClassificationDescriptions",
            "type": "System.String",
            "defaultValue": "",
            "description": "A comma-delimited list of structured strings describing the classification values in the ClassificationList. The structure of the string is: Value: Description"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->