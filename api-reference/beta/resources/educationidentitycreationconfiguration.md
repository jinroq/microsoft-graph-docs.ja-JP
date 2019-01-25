---
title: educationIdentityCreationConfiguration リソースの種類
description: 学校データ プロファイル id の作成時に設定を定義します。 これらの id には、生徒と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリに作成されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 92ad3c36a9379bb570f2a635038903e64a0309e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511402"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a><span data-ttu-id="acea4-105">educationIdentityCreationConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="acea4-105">educationIdentityCreationConfiguration resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acea4-106">学校データ プロファイル id の作成時に設定を定義します。</span><span class="sxs-lookup"><span data-stu-id="acea4-106">Defines the settings on creation of school data profile identities.</span></span> <span data-ttu-id="acea4-107">これらの id には、生徒と教師が含まれます。</span><span class="sxs-lookup"><span data-stu-id="acea4-107">These identities include students and teachers.</span></span> <span data-ttu-id="acea4-108">これらの設定に基づいて、ユーザーがディレクトリに作成されます。</span><span class="sxs-lookup"><span data-stu-id="acea4-108">Based on these settings, the users will be created in the directory.</span></span>

> <span data-ttu-id="acea4-109">**注:** ディレクトリ同期がオンになって、設置型の間で同期する Active Directory と Azure Active Directory (AD の Azure) を使っている場合は、 [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md)のリソースを使用してください。</span><span class="sxs-lookup"><span data-stu-id="acea4-109">**Note:** If you have directory sync turned on to sync between on-premises Active Directory and Azure Active Directory (Azure AD), use the [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md) resource instead.</span></span>

<span data-ttu-id="acea4-110">[EducationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="acea4-110">Derived from [educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="acea4-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="acea4-111">Properties</span></span>

| <span data-ttu-id="acea4-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="acea4-112">Property</span></span> | <span data-ttu-id="acea4-113">型</span><span class="sxs-lookup"><span data-stu-id="acea4-113">Type</span></span> | <span data-ttu-id="acea4-114">説明</span><span class="sxs-lookup"><span data-stu-id="acea4-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="acea4-115">**userDomains**</span><span class="sxs-lookup"><span data-stu-id="acea4-115">**userDomains**</span></span> | <span data-ttu-id="acea4-116">[educationIdentityDomain](educationidentitydomain.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="acea4-116">[educationIdentityDomain](educationidentitydomain.md) collection</span></span> |  <span data-ttu-id="acea4-117">ユーザーの種類ごとに使用するドメインの一覧を設定します。</span><span class="sxs-lookup"><span data-stu-id="acea4-117">Sets the list of domains to use per user type.</span></span>  |


## <a name="json-representation"></a><span data-ttu-id="acea4-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="acea4-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "microsoft.graph.educationIdentityDomain",
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitycreationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
