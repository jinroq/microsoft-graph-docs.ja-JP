---
title: mfaDetail リソースの種類
description: '特定のサインインの MFA の詳細を示します。 サインインで認証の詳細と、使用する認証方法が含まれています (例: 電話、SMS、またはボイス メール) '
localization_priority: Normal
ms.openlocfilehash: 5069045fd202d443a94a80f7333f12ab5e707ada
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883742"
---
# <a name="mfadetail-resource-type"></a><span data-ttu-id="574b1-104">mfaDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="574b1-104">mfaDetail resource type</span></span>
<span data-ttu-id="574b1-105">特定のサインインの MFA の詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="574b1-105">Indicates MFA details for a specific sign-in.</span></span> <span data-ttu-id="574b1-106">サインインで認証の詳細と、使用する認証方法が含まれています (例: 電話、SMS、またはボイス メール)</span><span class="sxs-lookup"><span data-stu-id="574b1-106">It includes the authentication method used for signing in as well as auth details (for example: Phone, SMS or voicemail)</span></span> 



## <a name="properties"></a><span data-ttu-id="574b1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="574b1-107">Properties</span></span>
| <span data-ttu-id="574b1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="574b1-108">Property</span></span>     | <span data-ttu-id="574b1-109">種類</span><span class="sxs-lookup"><span data-stu-id="574b1-109">Type</span></span>   |<span data-ttu-id="574b1-110">説明</span><span class="sxs-lookup"><span data-stu-id="574b1-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="574b1-111">authDetail</span><span class="sxs-lookup"><span data-stu-id="574b1-111">authDetail</span></span>|<span data-ttu-id="574b1-112">String</span><span class="sxs-lookup"><span data-stu-id="574b1-112">String</span></span>|<span data-ttu-id="574b1-113">必要な MFA は、[はい] とは、対応する記号の活動の MFA の認証の詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="574b1-113">Indicates the MFA auth detail for the corresponding Sign-in activity when the MFA Required is "Yes".</span></span>|
|<span data-ttu-id="574b1-114">authMethod</span><span class="sxs-lookup"><span data-stu-id="574b1-114">authMethod</span></span>|<span data-ttu-id="574b1-115">String</span><span class="sxs-lookup"><span data-stu-id="574b1-115">String</span></span>|<span data-ttu-id="574b1-116">MFA のために必要なフィールドは、[はい] をするときに、対応する記号の活動の MFA の認証方法 (SMS、電話、ユーザー認証システムのアプリケーションは、いくつかの値) を示します。</span><span class="sxs-lookup"><span data-stu-id="574b1-116">Indicates the MFA Auth methods (SMS, Phone, Authenticator App are some of the value) for the corresponding sign-in activity when the MFA Required field is "Yes".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="574b1-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="574b1-117">JSON representation</span></span>

<span data-ttu-id="574b1-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="574b1-118">Here is a JSON representation of the resource.</span></span>

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
