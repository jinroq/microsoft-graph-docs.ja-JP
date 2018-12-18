---
title: customSubjectAlternativeName リソースの種類
description: カスタムのサブジェクトの別名定義
author: tfitzmac
ms.openlocfilehash: 5ed3f62cef38340ae7204b98e1fc984ba9bcb9cc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349316"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="022c7-103">customSubjectAlternativeName リソースの種類</span><span class="sxs-lookup"><span data-stu-id="022c7-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="022c7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="022c7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="022c7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="022c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="022c7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="022c7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="022c7-107">カスタムのサブジェクトの別名定義</span><span class="sxs-lookup"><span data-stu-id="022c7-107">Custom Subject Alternative Name definition</span></span>
## <a name="properties"></a><span data-ttu-id="022c7-108">Properties</span><span class="sxs-lookup"><span data-stu-id="022c7-108">Properties</span></span>
|<span data-ttu-id="022c7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="022c7-109">Property</span></span>|<span data-ttu-id="022c7-110">種類</span><span class="sxs-lookup"><span data-stu-id="022c7-110">Type</span></span>|<span data-ttu-id="022c7-111">説明</span><span class="sxs-lookup"><span data-stu-id="022c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="022c7-112">sanType</span><span class="sxs-lookup"><span data-stu-id="022c7-112">sanType</span></span>|[<span data-ttu-id="022c7-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="022c7-113">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="022c7-114">SAN のカスタム型です。</span><span class="sxs-lookup"><span data-stu-id="022c7-114">Custom SAN Type.</span></span> <span data-ttu-id="022c7-115">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="022c7-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="022c7-116">名前</span><span class="sxs-lookup"><span data-stu-id="022c7-116">name</span></span>|<span data-ttu-id="022c7-117">String</span><span class="sxs-lookup"><span data-stu-id="022c7-117">String</span></span>|<span data-ttu-id="022c7-118">SAN のカスタム名</span><span class="sxs-lookup"><span data-stu-id="022c7-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="022c7-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="022c7-119">Relationships</span></span>
<span data-ttu-id="022c7-120">なし</span><span class="sxs-lookup"><span data-stu-id="022c7-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="022c7-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="022c7-121">JSON Representation</span></span>
<span data-ttu-id="022c7-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="022c7-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```





