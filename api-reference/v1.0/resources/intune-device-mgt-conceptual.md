---
title: Microsoft Intune でのデバイス管理
description: ''
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3d665b70f812a18f840ce43a029fe0729d454745
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980644"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="d10d3-102">Microsoft Intune でのデバイス管理</span><span class="sxs-lookup"><span data-stu-id="d10d3-102">Device management in Microsoft Intune</span></span>

> <span data-ttu-id="d10d3-103">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d10d3-103">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="d10d3-104">動作状態</span><span class="sxs-lookup"><span data-stu-id="d10d3-104">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="d10d3-105">Apple プッシュ通知証明書</span><span class="sxs-lookup"><span data-stu-id="d10d3-105">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="d10d3-106">監査アクター</span><span class="sxs-lookup"><span data-stu-id="d10d3-106">Audit actor</span></span>](intune-auditing-auditactor.md)
- [<span data-ttu-id="d10d3-107">監査イベント</span><span class="sxs-lookup"><span data-stu-id="d10d3-107">Audit event</span></span>](intune-auditing-auditevent.md)
- [<span data-ttu-id="d10d3-108">監査のプロパティ</span><span class="sxs-lookup"><span data-stu-id="d10d3-108">Audit property</span></span>](intune-auditing-auditproperty.md)
- [<span data-ttu-id="d10d3-109">監査のリソース</span><span class="sxs-lookup"><span data-stu-id="d10d3-109">Audit resource</span></span>](intune-auditing-auditresource.md)
- [<span data-ttu-id="d10d3-110">準拠状態</span><span class="sxs-lookup"><span data-stu-id="d10d3-110">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="d10d3-111">構成マネージャーのクライアントに対応した機能</span><span class="sxs-lookup"><span data-stu-id="d10d3-111">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="d10d3-112">共有の Apple デバイスのアクションの結果からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="d10d3-112">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="d10d3-113">検出されたアプリ</span><span class="sxs-lookup"><span data-stu-id="d10d3-113">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="d10d3-114">デバイスのアクションの結果</span><span class="sxs-lookup"><span data-stu-id="d10d3-114">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="d10d3-115">デバイス登録の失敗の理由</span><span class="sxs-lookup"><span data-stu-id="d10d3-115">Device enrollment failure reason</span></span>](intune-troubleshooting-deviceenrollmentfailurereason.md)
- [<span data-ttu-id="d10d3-116">デバイス登録の種類</span><span class="sxs-lookup"><span data-stu-id="d10d3-116">Device enrollment type</span></span>](intune-devices-deviceenrollmenttype.md)
- [<span data-ttu-id="d10d3-117">デバイスの Exchange アクセス状態の要約</span><span class="sxs-lookup"><span data-stu-id="d10d3-117">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="d10d3-118">デバイスの位置情報</span><span class="sxs-lookup"><span data-stu-id="d10d3-118">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="d10d3-119">デバイスの正常性構成証明の状態</span><span class="sxs-lookup"><span data-stu-id="d10d3-119">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="d10d3-120">デバイス管理 exchange のアクセスの状態</span><span class="sxs-lookup"><span data-stu-id="d10d3-120">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="d10d3-121">デバイス管理 exchange アクセス状態の理由</span><span class="sxs-lookup"><span data-stu-id="d10d3-121">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="d10d3-122">デバイス管理のサブスクリプションの状態</span><span class="sxs-lookup"><span data-stu-id="d10d3-122">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="d10d3-123">デバイス管理のトラブルシューティング イベント</span><span class="sxs-lookup"><span data-stu-id="d10d3-123">Device management troubleshooting event</span></span>](intune-troubleshooting-devicemanagementtroubleshootingevent.md)
- [<span data-ttu-id="d10d3-124">デバイスのオペレーティング システムの概要</span><span class="sxs-lookup"><span data-stu-id="d10d3-124">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="d10d3-125">デバイス登録の状態</span><span class="sxs-lookup"><span data-stu-id="d10d3-125">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="d10d3-126">登録のトラブルシューティング イベント</span><span class="sxs-lookup"><span data-stu-id="d10d3-126">Enrollment troubleshooting event</span></span>](intune-troubleshooting-enrollmenttroubleshootingevent.md)
- [<span data-ttu-id="d10d3-127">ローカライズ済み通知メッセージ</span><span class="sxs-lookup"><span data-stu-id="d10d3-127">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="d10d3-128">デバイスの検索アクションの結果</span><span class="sxs-lookup"><span data-stu-id="d10d3-128">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="d10d3-129">管理対象デバイス</span><span class="sxs-lookup"><span data-stu-id="d10d3-129">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="d10d3-130">管理対象デバイスの概要</span><span class="sxs-lookup"><span data-stu-id="d10d3-130">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="d10d3-131">デバイス所有者の種類を管理</span><span class="sxs-lookup"><span data-stu-id="d10d3-131">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="d10d3-132">管理対象デバイスのパートナーは、正常性状態を報告</span><span class="sxs-lookup"><span data-stu-id="d10d3-132">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="d10d3-133">管理エージェントの種類</span><span class="sxs-lookup"><span data-stu-id="d10d3-133">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="d10d3-134">通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="d10d3-134">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="d10d3-135">通知テンプレートのオプションをブランド化</span><span class="sxs-lookup"><span data-stu-id="d10d3-135">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="d10d3-136">リモート アシスタンスの採用状況</span><span class="sxs-lookup"><span data-stu-id="d10d3-136">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="d10d3-137">リモート アシスタンス パートナー</span><span class="sxs-lookup"><span data-stu-id="d10d3-137">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="d10d3-138">リモート ロック アクションの結果</span><span class="sxs-lookup"><span data-stu-id="d10d3-138">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="d10d3-139">パスコードのリセット アクションの結果</span><span class="sxs-lookup"><span data-stu-id="d10d3-139">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="d10d3-140">Windows のデバイス アカウントのアクション パラメーターの更新</span><span class="sxs-lookup"><span data-stu-id="d10d3-140">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="d10d3-141">Windows Defender のスキャン アクションの結果</span><span class="sxs-lookup"><span data-stu-id="d10d3-141">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="d10d3-142">Windows のデバイス アカウント</span><span class="sxs-lookup"><span data-stu-id="d10d3-142">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="d10d3-143">Windows のデバイス AD アカウント</span><span class="sxs-lookup"><span data-stu-id="d10d3-143">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="d10d3-144">Windows のデバイス Azure AD アカウント</span><span class="sxs-lookup"><span data-stu-id="d10d3-144">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)
