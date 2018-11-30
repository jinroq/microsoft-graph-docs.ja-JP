---
title: win32LobAppInstallExperience リソースの種類
description: Win32 アプリケーションのインストール環境のプロパティが含まれています
ms.openlocfilehash: 04fed453125155073d75de417d13cfd81a5bcdd1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067616"
---
# <a name="win32lobappinstallexperience-resource-type"></a><span data-ttu-id="bff3c-103">win32LobAppInstallExperience リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bff3c-103">win32LobAppInstallExperience resource type</span></span>

> <span data-ttu-id="bff3c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bff3c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bff3c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bff3c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bff3c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bff3c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bff3c-107">Win32 アプリケーションのインストール環境のプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="bff3c-107">Contains installation experience properties for a Win32 App</span></span>
## <a name="properties"></a><span data-ttu-id="bff3c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bff3c-108">Properties</span></span>
|<span data-ttu-id="bff3c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bff3c-109">Property</span></span>|<span data-ttu-id="bff3c-110">型</span><span class="sxs-lookup"><span data-stu-id="bff3c-110">Type</span></span>|<span data-ttu-id="bff3c-111">説明</span><span class="sxs-lookup"><span data-stu-id="bff3c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bff3c-112">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="bff3c-112">runAsAccount</span></span>|[<span data-ttu-id="bff3c-113">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="bff3c-113">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="bff3c-114">アプリケーションが実行される実行コンテキストの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="bff3c-114">Indicates the type of execution context the app runs in.</span></span> <span data-ttu-id="bff3c-115">可能な値: `system`、`user`。</span><span class="sxs-lookup"><span data-stu-id="bff3c-115">Possible values are: `system`, `user`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bff3c-116">関係</span><span class="sxs-lookup"><span data-stu-id="bff3c-116">Relationships</span></span>
<span data-ttu-id="bff3c-117">なし</span><span class="sxs-lookup"><span data-stu-id="bff3c-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bff3c-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bff3c-118">JSON Representation</span></span>
<span data-ttu-id="bff3c-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bff3c-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppInstallExperience",
  "runAsAccount": "String"
}
```





