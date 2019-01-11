---
title: windowsEnrollmentStatusScreenSettings リソースの種類
description: 登録ステータス画面の設定
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7263fdd8ab3d9a39d5081322c62cfcf76a4c7aa0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877449"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="b3006-103">windowsEnrollmentStatusScreenSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b3006-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

> <span data-ttu-id="b3006-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b3006-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3006-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3006-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3006-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b3006-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3006-107">登録ステータス画面の設定</span><span class="sxs-lookup"><span data-stu-id="b3006-107">Enrollment status screen setting</span></span>
## <a name="properties"></a><span data-ttu-id="b3006-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3006-108">Properties</span></span>
|<span data-ttu-id="b3006-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3006-109">Property</span></span>|<span data-ttu-id="b3006-110">種類</span><span class="sxs-lookup"><span data-stu-id="b3006-110">Type</span></span>|<span data-ttu-id="b3006-111">説明</span><span class="sxs-lookup"><span data-stu-id="b3006-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3006-112">hideInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="b3006-112">hideInstallationProgress</span></span>|<span data-ttu-id="b3006-113">ブール型</span><span class="sxs-lookup"><span data-stu-id="b3006-113">Boolean</span></span>|<span data-ttu-id="b3006-114">ユーザーにインストールの進行状況の表示と非表示を切り替える</span><span class="sxs-lookup"><span data-stu-id="b3006-114">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="b3006-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span><span class="sxs-lookup"><span data-stu-id="b3006-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="b3006-116">ブール型</span><span class="sxs-lookup"><span data-stu-id="b3006-116">Boolean</span></span>|<span data-ttu-id="b3006-117">許可またはブロックのユーザー プロファイル、およびアプリケーション インストールが完了する前にデバイスを使用するには</span><span class="sxs-lookup"><span data-stu-id="b3006-117">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="b3006-118">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="b3006-118">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="b3006-119">ブール型</span><span class="sxs-lookup"><span data-stu-id="b3006-119">Boolean</span></span>|<span data-ttu-id="b3006-120">インストールの失敗時にセットアップを再実行するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="b3006-120">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="b3006-121">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="b3006-121">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="b3006-122">ブール型</span><span class="sxs-lookup"><span data-stu-id="b3006-122">Boolean</span></span>|<span data-ttu-id="b3006-123">許可またはブロックのインストールの失敗時にログの収集</span><span class="sxs-lookup"><span data-stu-id="b3006-123">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="b3006-124">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="b3006-124">customErrorMessage</span></span>|<span data-ttu-id="b3006-125">String</span><span class="sxs-lookup"><span data-stu-id="b3006-125">String</span></span>|<span data-ttu-id="b3006-126">インストールの失敗時に表示するカスタム エラー メッセージを設定します。</span><span class="sxs-lookup"><span data-stu-id="b3006-126">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="b3006-127">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="b3006-127">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="b3006-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b3006-128">Int32</span></span>|<span data-ttu-id="b3006-129">インストールの進行状況のタイムアウトを分単位で設定します。</span><span class="sxs-lookup"><span data-stu-id="b3006-129">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="b3006-130">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="b3006-130">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="b3006-131">ブール型</span><span class="sxs-lookup"><span data-stu-id="b3006-131">Boolean</span></span>|<span data-ttu-id="b3006-132">インストールの失敗時にデバイスを使用するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="b3006-132">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3006-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b3006-133">Relationships</span></span>
<span data-ttu-id="b3006-134">なし</span><span class="sxs-lookup"><span data-stu-id="b3006-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b3006-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b3006-135">JSON Representation</span></span>
<span data-ttu-id="b3006-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b3006-136">Here is a JSON representation of the resource.</span></span>
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





