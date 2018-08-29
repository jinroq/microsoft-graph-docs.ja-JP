# <a name="passwordprofile-resource-type"></a><span data-ttu-id="6ffd7-101">passwordProfile リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6ffd7-101">passwordProfile resource type</span></span>

<span data-ttu-id="6ffd7-p101">ユーザーに関連付けられているパスワードのプロファイルが含まれています。[ユーザー](user.md) エンティティの **PasswordProfile** プロパティは、**passwordProfile** オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6ffd7-p101">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="6ffd7-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ffd7-104">Properties</span></span>
| <span data-ttu-id="6ffd7-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ffd7-105">Property</span></span>     | <span data-ttu-id="6ffd7-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="6ffd7-106">Type</span></span>   |<span data-ttu-id="6ffd7-107">説明</span><span class="sxs-lookup"><span data-stu-id="6ffd7-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ffd7-108">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="6ffd7-108">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="6ffd7-109">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ffd7-109">Boolean</span></span>| <span data-ttu-id="6ffd7-110">ユーザーが次回のログインでパスワードを変更する必要がある場合は **true**、それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="6ffd7-110">**true** if the user must change her password on the next login; otherwise **false**.</span></span> |
|<span data-ttu-id="6ffd7-111">password</span><span class="sxs-lookup"><span data-stu-id="6ffd7-111">password</span></span>|<span data-ttu-id="6ffd7-112">String</span><span class="sxs-lookup"><span data-stu-id="6ffd7-112">String</span></span>|<span data-ttu-id="6ffd7-p102">ユーザーのパスワード。このプロパティは、ユーザーの作成時に必要です。このプロパティは更新できますが、ユーザーは次回のログインでパスワードを変更する必要があります。パスワードは、ユーザーの **passwordPolicies** プロパティによって指定されているとおりの最小要件を満たす必要があります。既定では、強力なパスワードが必要です。</span><span class="sxs-lookup"><span data-stu-id="6ffd7-p102">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6ffd7-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6ffd7-118">JSON representation</span></span>

<span data-ttu-id="6ffd7-119">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="6ffd7-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordProfile"
}-->

```json
{
  "forceChangePasswordNextSignIn": true,
  "password": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->