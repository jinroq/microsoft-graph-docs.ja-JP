    ---
<span data-ttu-id="00539-101">title: "educationIdentitySynchronizationConfiguration resource type" description: "すべての学校データプロファイル id 同期構成の抽象基本クラス。</span><span class="sxs-lookup"><span data-stu-id="00539-101">title: "educationIdentitySynchronizationConfiguration resource type" description: "Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="00539-102">派生クラスは、id を同期するための動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="00539-102">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="00539-103">派生型の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="00539-103">The following are the derived types."</span></span>
<span data-ttu-id="00539-104">著者: "mmast-msft" 送受信: 通常の ms 製品: "教育"</span><span class="sxs-lookup"><span data-stu-id="00539-104">author: "mmast-msft" localization_priority: Normal ms.prod: "education"</span></span>
---

# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="00539-105">educationIdentitySynchronizationConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="00539-105">educationIdentitySynchronizationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00539-106">すべての学校データプロファイル id 同期構成の抽象基本クラス。</span><span class="sxs-lookup"><span data-stu-id="00539-106">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="00539-107">派生クラスは、id を同期するための動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="00539-107">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="00539-108">派生型を次に示します。</span><span class="sxs-lookup"><span data-stu-id="00539-108">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="00539-109">派生型</span><span class="sxs-lookup"><span data-stu-id="00539-109">Derived types</span></span>
| <span data-ttu-id="00539-110">型</span><span class="sxs-lookup"><span data-stu-id="00539-110">Type</span></span> | <span data-ttu-id="00539-111">説明</span><span class="sxs-lookup"><span data-stu-id="00539-111">Description</span></span> |
|:-|:-|
| [<span data-ttu-id="00539-112">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="00539-112">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="00539-113">この種類を使用して、azure Active Directory (azure AD) の既存のユーザーアカウントと照合します。</span><span class="sxs-lookup"><span data-stu-id="00539-113">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="00539-114">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="00539-114">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="00539-115">この種類を使用して、Azure AD で新しいユーザーアカウントを作成します。</span><span class="sxs-lookup"><span data-stu-id="00539-115">Use this type to create new user accounts in Azure AD.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="00539-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="00539-116">JSON representation</span></span>
<!-- {
  "blockType": "resource",
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{
}
```

