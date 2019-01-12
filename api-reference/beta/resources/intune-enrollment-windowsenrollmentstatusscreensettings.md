---
title: windowsEnrollmentStatusScreenSettings リソースの種類
description: 登録ステータス画面の設定
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: abc48a1d63cc514d2ec887a7758e69a0ea8112a7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978572"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="61eb1-103">windowsEnrollmentStatusScreenSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="61eb1-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

> <span data-ttu-id="61eb1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="61eb1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="61eb1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61eb1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="61eb1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="61eb1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61eb1-107">登録ステータス画面の設定</span><span class="sxs-lookup"><span data-stu-id="61eb1-107">Enrollment status screen setting</span></span>
## <a name="properties"></a><span data-ttu-id="61eb1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61eb1-108">Properties</span></span>
|<span data-ttu-id="61eb1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61eb1-109">Property</span></span>|<span data-ttu-id="61eb1-110">型</span><span class="sxs-lookup"><span data-stu-id="61eb1-110">Type</span></span>|<span data-ttu-id="61eb1-111">説明</span><span class="sxs-lookup"><span data-stu-id="61eb1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61eb1-112">hideInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="61eb1-112">hideInstallationProgress</span></span>|<span data-ttu-id="61eb1-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="61eb1-113">Boolean</span></span>|<span data-ttu-id="61eb1-114">ユーザーにインストールの進行状況の表示と非表示を切り替える</span><span class="sxs-lookup"><span data-stu-id="61eb1-114">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="61eb1-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span><span class="sxs-lookup"><span data-stu-id="61eb1-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="61eb1-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="61eb1-116">Boolean</span></span>|<span data-ttu-id="61eb1-117">許可またはブロックのユーザー プロファイル、およびアプリケーション インストールが完了する前にデバイスを使用するには</span><span class="sxs-lookup"><span data-stu-id="61eb1-117">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="61eb1-118">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="61eb1-118">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="61eb1-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="61eb1-119">Boolean</span></span>|<span data-ttu-id="61eb1-120">インストールの失敗時にセットアップを再実行するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="61eb1-120">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="61eb1-121">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="61eb1-121">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="61eb1-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="61eb1-122">Boolean</span></span>|<span data-ttu-id="61eb1-123">許可またはブロックのインストールの失敗時にログの収集</span><span class="sxs-lookup"><span data-stu-id="61eb1-123">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="61eb1-124">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="61eb1-124">customErrorMessage</span></span>|<span data-ttu-id="61eb1-125">String</span><span class="sxs-lookup"><span data-stu-id="61eb1-125">String</span></span>|<span data-ttu-id="61eb1-126">インストールの失敗時に表示するカスタム エラー メッセージを設定します。</span><span class="sxs-lookup"><span data-stu-id="61eb1-126">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="61eb1-127">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="61eb1-127">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="61eb1-128">Int32</span><span class="sxs-lookup"><span data-stu-id="61eb1-128">Int32</span></span>|<span data-ttu-id="61eb1-129">インストールの進行状況のタイムアウトを分単位で設定します。</span><span class="sxs-lookup"><span data-stu-id="61eb1-129">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="61eb1-130">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="61eb1-130">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="61eb1-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="61eb1-131">Boolean</span></span>|<span data-ttu-id="61eb1-132">インストールの失敗時にデバイスを使用するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="61eb1-132">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="61eb1-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="61eb1-133">Relationships</span></span>
<span data-ttu-id="61eb1-134">なし</span><span class="sxs-lookup"><span data-stu-id="61eb1-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="61eb1-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="61eb1-135">JSON Representation</span></span>
<span data-ttu-id="61eb1-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="61eb1-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsEnrollmentStatusScreenSettings",
  "hideInstallationProgress": true,
  "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
  "blockDeviceSetupRetryByUser": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "String",
  "installProgressTimeoutInMinutes": 1024,
  "allowDeviceUseOnInstallFailure": true
}
```





