---
title: bitLockerRemovableDrivePolicy リソースの種類
description: BitLocker リムーバブル ドライブ ポリシー。
author: tfitzmac
ms.openlocfilehash: 15de11384195350b455cd4696a260aedf1de7a26
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354035"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="b3d39-103">bitLockerRemovableDrivePolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b3d39-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="b3d39-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b3d39-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3d39-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3d39-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3d39-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b3d39-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3d39-107">BitLocker リムーバブル ドライブ ポリシー。</span><span class="sxs-lookup"><span data-stu-id="b3d39-107">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="b3d39-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3d39-108">Properties</span></span>
|<span data-ttu-id="b3d39-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3d39-109">Property</span></span>|<span data-ttu-id="b3d39-110">種類</span><span class="sxs-lookup"><span data-stu-id="b3d39-110">Type</span></span>|<span data-ttu-id="b3d39-111">説明</span><span class="sxs-lookup"><span data-stu-id="b3d39-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3d39-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="b3d39-112">encryptionMethod</span></span>|[<span data-ttu-id="b3d39-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="b3d39-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="b3d39-114">リムーバブル ドライブの暗号化方法を選択します。</span><span class="sxs-lookup"><span data-stu-id="b3d39-114">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="b3d39-115">可能な値は、`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256` です。</span><span class="sxs-lookup"><span data-stu-id="b3d39-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="b3d39-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="b3d39-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="b3d39-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3d39-117">Boolean</span></span>|<span data-ttu-id="b3d39-118">別の組織で構成されたデバイスへの書き込みアクセスをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b3d39-118">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="b3d39-119">RequireEncryptionForWriteAccess が false の場合、この値は影響を与えません。</span><span class="sxs-lookup"><span data-stu-id="b3d39-119">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="b3d39-120">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="b3d39-120">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="b3d39-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3d39-121">Boolean</span></span>|<span data-ttu-id="b3d39-122">このポリシー設定は、コンピューター上でリムーバブル データ ドライブを書き込み可能にする際に、BitLocker 保護が必要かどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="b3d39-122">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3d39-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b3d39-123">Relationships</span></span>
<span data-ttu-id="b3d39-124">なし</span><span class="sxs-lookup"><span data-stu-id="b3d39-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b3d39-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b3d39-125">JSON Representation</span></span>
<span data-ttu-id="b3d39-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b3d39-126">Here is a JSON representation of the resource.</span></span>
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





