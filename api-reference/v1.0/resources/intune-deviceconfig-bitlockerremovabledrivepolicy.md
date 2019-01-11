---
title: bitLockerRemovableDrivePolicy リソースの種類
description: BitLocker リムーバブル ドライブ ポリシー。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fc9fe3350fd9f4b5c5808de2c35fa3451943e449
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830836"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="5318b-103">bitLockerRemovableDrivePolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5318b-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="5318b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5318b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5318b-105">BitLocker リムーバブル ドライブ ポリシー。</span><span class="sxs-lookup"><span data-stu-id="5318b-105">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="5318b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5318b-106">Properties</span></span>
|<span data-ttu-id="5318b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5318b-107">Property</span></span>|<span data-ttu-id="5318b-108">種類</span><span class="sxs-lookup"><span data-stu-id="5318b-108">Type</span></span>|<span data-ttu-id="5318b-109">説明</span><span class="sxs-lookup"><span data-stu-id="5318b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5318b-110">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="5318b-110">encryptionMethod</span></span>|[<span data-ttu-id="5318b-111">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="5318b-111">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="5318b-112">リムーバブル ドライブの暗号化方法を選択します。</span><span class="sxs-lookup"><span data-stu-id="5318b-112">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="5318b-113">可能な値は、`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256` です。</span><span class="sxs-lookup"><span data-stu-id="5318b-113">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="5318b-114">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="5318b-114">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="5318b-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="5318b-115">Boolean</span></span>|<span data-ttu-id="5318b-116">別の組織で構成されたデバイスへの書き込みアクセスをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5318b-116">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="5318b-117">RequireEncryptionForWriteAccess が false の場合、この値は影響を与えません。</span><span class="sxs-lookup"><span data-stu-id="5318b-117">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="5318b-118">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="5318b-118">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="5318b-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="5318b-119">Boolean</span></span>|<span data-ttu-id="5318b-120">このポリシー設定は、コンピューター上でリムーバブル データ ドライブを書き込み可能にする際に、BitLocker 保護が必要かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="5318b-120">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5318b-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5318b-121">Relationships</span></span>
<span data-ttu-id="5318b-122">なし</span><span class="sxs-lookup"><span data-stu-id="5318b-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5318b-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5318b-123">JSON Representation</span></span>
<span data-ttu-id="5318b-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5318b-124">Here is a JSON representation of the resource.</span></span>
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



