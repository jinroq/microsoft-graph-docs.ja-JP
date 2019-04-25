---
title: mfadetail リソースの種類
description: '特定のサインインの MFA の詳細を示します。 これには、サインインと認証の詳細 (たとえば、電話、SMS、ボイスメール) に使用される認証方法が含まれています。 '
localization_priority: Normal
ms.openlocfilehash: 5069045fd202d443a94a80f7333f12ab5e707ada
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581479"
---
# <a name="mfadetail-resource-type"></a><span data-ttu-id="0a931-104">mfadetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0a931-104">mfaDetail resource type</span></span>
<span data-ttu-id="0a931-105">特定のサインインの MFA の詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="0a931-105">Indicates MFA details for a specific sign-in.</span></span> <span data-ttu-id="0a931-106">これには、サインインと認証の詳細 (たとえば、電話、SMS、ボイスメール) に使用される認証方法が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0a931-106">It includes the authentication method used for signing in as well as auth details (for example: Phone, SMS or voicemail)</span></span> 



## <a name="properties"></a><span data-ttu-id="0a931-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a931-107">Properties</span></span>
| <span data-ttu-id="0a931-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a931-108">Property</span></span>     | <span data-ttu-id="0a931-109">型</span><span class="sxs-lookup"><span data-stu-id="0a931-109">Type</span></span>   |<span data-ttu-id="0a931-110">説明</span><span class="sxs-lookup"><span data-stu-id="0a931-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a931-111">authdetail</span><span class="sxs-lookup"><span data-stu-id="0a931-111">authDetail</span></span>|<span data-ttu-id="0a931-112">String</span><span class="sxs-lookup"><span data-stu-id="0a931-112">String</span></span>|<span data-ttu-id="0a931-113">mfa が必須である、対応するサインインアクティビティの mfa 認証詳細が "Yes" であることを示します。</span><span class="sxs-lookup"><span data-stu-id="0a931-113">Indicates the MFA auth detail for the corresponding Sign-in activity when the MFA Required is "Yes".</span></span>|
|<span data-ttu-id="0a931-114">authmethod</span><span class="sxs-lookup"><span data-stu-id="0a931-114">authMethod</span></span>|<span data-ttu-id="0a931-115">String</span><span class="sxs-lookup"><span data-stu-id="0a931-115">String</span></span>|<span data-ttu-id="0a931-116">mfa 必須フィールドが "Yes" の場合に、対応するサインインアクティビティの mfa 認証方法 (SMS、Phone、Authenticator アプリ) を示します。</span><span class="sxs-lookup"><span data-stu-id="0a931-116">Indicates the MFA Auth methods (SMS, Phone, Authenticator App are some of the value) for the corresponding sign-in activity when the MFA Required field is "Yes".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a931-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0a931-117">JSON representation</span></span>

<span data-ttu-id="0a931-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0a931-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mfaDetail"
}-->

```json
{
  "authDetail": "String",
  "authMethod": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mfaDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
