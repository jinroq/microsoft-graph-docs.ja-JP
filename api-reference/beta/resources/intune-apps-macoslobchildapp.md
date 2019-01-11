---
title: macOSLobChildApp リソースの種類
description: バンドル パッケージに MacOS の LOB アプリケーションのプロパティが含まれています
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2fd4440422ee184b62da4731f49ead4316a2fa45
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851248"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="8c355-103">macOSLobChildApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8c355-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="8c355-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8c355-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c355-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c355-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c355-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8c355-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c355-107">バンドル パッケージに MacOS の LOB アプリケーションのプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="8c355-107">Contains properties the MacOS LOB App in a bundle package</span></span>
## <a name="properties"></a><span data-ttu-id="8c355-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c355-108">Properties</span></span>
|<span data-ttu-id="8c355-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c355-109">Property</span></span>|<span data-ttu-id="8c355-110">種類</span><span class="sxs-lookup"><span data-stu-id="8c355-110">Type</span></span>|<span data-ttu-id="8c355-111">説明</span><span class="sxs-lookup"><span data-stu-id="8c355-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c355-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="8c355-112">bundleId</span></span>|<span data-ttu-id="8c355-113">String</span><span class="sxs-lookup"><span data-stu-id="8c355-113">String</span></span>|<span data-ttu-id="8c355-114">ID 名。</span><span class="sxs-lookup"><span data-stu-id="8c355-114">The Identity Name.</span></span>|
|<span data-ttu-id="8c355-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="8c355-115">buildNumber</span></span>|<span data-ttu-id="8c355-116">String</span><span class="sxs-lookup"><span data-stu-id="8c355-116">String</span></span>|<span data-ttu-id="8c355-117">MacOS の基幹業務 (LoB) アプリケーションのビルド番号です。</span><span class="sxs-lookup"><span data-stu-id="8c355-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8c355-118">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="8c355-118">versionNumber</span></span>|<span data-ttu-id="8c355-119">String</span><span class="sxs-lookup"><span data-stu-id="8c355-119">String</span></span>|<span data-ttu-id="8c355-120">MacOS の基幹業務 (LoB) アプリケーションのバージョン番号です。</span><span class="sxs-lookup"><span data-stu-id="8c355-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c355-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8c355-121">Relationships</span></span>
<span data-ttu-id="8c355-122">なし</span><span class="sxs-lookup"><span data-stu-id="8c355-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8c355-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8c355-123">JSON Representation</span></span>
<span data-ttu-id="8c355-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8c355-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```





