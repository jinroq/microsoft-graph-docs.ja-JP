---
title: bitLockerRemovableDrivePolicy リソースの種類
description: BitLocker リムーバブル ドライブ ポリシー。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 95dded55228cd6779de84db1bd8da1b745791c39
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948115"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="93f0c-103">bitLockerRemovableDrivePolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="93f0c-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="93f0c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="93f0c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93f0c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="93f0c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="93f0c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="93f0c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="93f0c-107">BitLocker リムーバブル ドライブ ポリシー。</span><span class="sxs-lookup"><span data-stu-id="93f0c-107">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="93f0c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93f0c-108">Properties</span></span>
|<span data-ttu-id="93f0c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93f0c-109">Property</span></span>|<span data-ttu-id="93f0c-110">種類</span><span class="sxs-lookup"><span data-stu-id="93f0c-110">Type</span></span>|<span data-ttu-id="93f0c-111">説明</span><span class="sxs-lookup"><span data-stu-id="93f0c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93f0c-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="93f0c-112">encryptionMethod</span></span>|[<span data-ttu-id="93f0c-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="93f0c-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="93f0c-114">リムーバブル ドライブの暗号化方法を選択します。</span><span class="sxs-lookup"><span data-stu-id="93f0c-114">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="93f0c-115">可能な値は、`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256` です。</span><span class="sxs-lookup"><span data-stu-id="93f0c-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="93f0c-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="93f0c-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="93f0c-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="93f0c-117">Boolean</span></span>|<span data-ttu-id="93f0c-118">別の組織で構成されたデバイスへの書き込みアクセスをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="93f0c-118">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="93f0c-119">RequireEncryptionForWriteAccess が false の場合、この値は影響を与えません。</span><span class="sxs-lookup"><span data-stu-id="93f0c-119">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="93f0c-120">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="93f0c-120">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="93f0c-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="93f0c-121">Boolean</span></span>|<span data-ttu-id="93f0c-122">このポリシー設定は、コンピューター上でリムーバブル データ ドライブを書き込み可能にする際に、BitLocker 保護が必要かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="93f0c-122">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93f0c-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="93f0c-123">Relationships</span></span>
<span data-ttu-id="93f0c-124">なし</span><span class="sxs-lookup"><span data-stu-id="93f0c-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="93f0c-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="93f0c-125">JSON Representation</span></span>
<span data-ttu-id="93f0c-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="93f0c-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```





