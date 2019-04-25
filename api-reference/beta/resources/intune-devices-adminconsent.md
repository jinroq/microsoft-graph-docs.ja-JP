---
title: adminconsent リソースの種類
description: 管理者の同意情報。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b14eb19096a034612715081ae2e3dba25b5bb218
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534494"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="099e6-103">adminconsent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="099e6-103">adminConsent resource type</span></span>

> <span data-ttu-id="099e6-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="099e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="099e6-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="099e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="099e6-106">管理者の同意情報。</span><span class="sxs-lookup"><span data-stu-id="099e6-106">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="099e6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="099e6-107">Properties</span></span>
|<span data-ttu-id="099e6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="099e6-108">Property</span></span>|<span data-ttu-id="099e6-109">型</span><span class="sxs-lookup"><span data-stu-id="099e6-109">Type</span></span>|<span data-ttu-id="099e6-110">説明</span><span class="sxs-lookup"><span data-stu-id="099e6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="099e6-111">/sharepoint データの編集</span><span class="sxs-lookup"><span data-stu-id="099e6-111">shareAPNSData</span></span>|[<span data-ttu-id="099e6-112">adminconの状態</span><span class="sxs-lookup"><span data-stu-id="099e6-112">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="099e6-113">ユーザーとデバイスのデータを Apple に共有するための管理者の同意状態。</span><span class="sxs-lookup"><span data-stu-id="099e6-113">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="099e6-114">可能な値は、`notConfigured`、`granted`、`notGranted` です。</span><span class="sxs-lookup"><span data-stu-id="099e6-114">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="099e6-115">関係</span><span class="sxs-lookup"><span data-stu-id="099e6-115">Relationships</span></span>
<span data-ttu-id="099e6-116">なし</span><span class="sxs-lookup"><span data-stu-id="099e6-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="099e6-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="099e6-117">JSON Representation</span></span>
<span data-ttu-id="099e6-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="099e6-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String"
}
```





