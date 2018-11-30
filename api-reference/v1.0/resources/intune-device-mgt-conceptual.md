---
title: Microsoft Intune でのデバイス管理
description: ''
ms.openlocfilehash: db7cc57a7f7b4463de494d49d4400cd7a563abaf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023275"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="cb08e-102">Microsoft Intune でのデバイス管理</span><span class="sxs-lookup"><span data-stu-id="cb08e-102">Device management in Microsoft Intune</span></span>

> <span data-ttu-id="cb08e-103">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cb08e-103">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="cb08e-104">動作状態</span><span class="sxs-lookup"><span data-stu-id="cb08e-104">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="cb08e-105">Apple プッシュ通知証明書</span><span class="sxs-lookup"><span data-stu-id="cb08e-105">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="cb08e-106">監査アクター</span><span class="sxs-lookup"><span data-stu-id="cb08e-106">Audit actor</span></span>](intune-auditing-auditactor.md)
- [<span data-ttu-id="cb08e-107">監査イベント</span><span class="sxs-lookup"><span data-stu-id="cb08e-107">Audit event</span></span>](intune-auditing-auditevent.md)
- [<span data-ttu-id="cb08e-108">監査のプロパティ</span><span class="sxs-lookup"><span data-stu-id="cb08e-108">Audit property</span></span>](intune-auditing-auditproperty.md)
- [<span data-ttu-id="cb08e-109">監査のリソース</span><span class="sxs-lookup"><span data-stu-id="cb08e-109">Audit resource</span></span>](intune-auditing-auditresource.md)
- [<span data-ttu-id="cb08e-110">準拠状態</span><span class="sxs-lookup"><span data-stu-id="cb08e-110">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="cb08e-111">構成マネージャーのクライアントに対応した機能</span><span class="sxs-lookup"><span data-stu-id="cb08e-111">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="cb08e-112">共有の Apple デバイスのアクションの結果からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="cb08e-112">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="cb08e-113">検出されたアプリ</span><span class="sxs-lookup"><span data-stu-id="cb08e-113">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="cb08e-114">デバイスのアクションの結果</span><span class="sxs-lookup"><span data-stu-id="cb08e-114">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="cb08e-115">デバイス登録の失敗の理由</span><span class="sxs-lookup"><span data-stu-id="cb08e-115">Device enrollment failure reason</span></span>](intune-troubleshooting-deviceenrollmentfailurereason.md)
- [<span data-ttu-id="cb08e-116">デバイス登録の種類</span><span class="sxs-lookup"><span data-stu-id="cb08e-116">Device enrollment type</span></span>](intune-devices-deviceenrollmenttype.md)
- [<span data-ttu-id="cb08e-117">デバイスの Exchange アクセス状態の要約</span><span class="sxs-lookup"><span data-stu-id="cb08e-117">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="cb08e-118">デバイスの位置情報</span><span class="sxs-lookup"><span data-stu-id="cb08e-118">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="cb08e-119">デバイスの正常性構成証明の状態</span><span class="sxs-lookup"><span data-stu-id="cb08e-119">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="cb08e-120">デバイス管理 exchange のアクセスの状態</span><span class="sxs-lookup"><span data-stu-id="cb08e-120">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="cb08e-121">デバイス管理 exchange アクセス状態の理由</span><span class="sxs-lookup"><span data-stu-id="cb08e-121">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="cb08e-122">デバイス管理のサブスクリプションの状態</span><span class="sxs-lookup"><span data-stu-id="cb08e-122">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="cb08e-123">デバイス管理のトラブルシューティング イベント</span><span class="sxs-lookup"><span data-stu-id="cb08e-123">Device management troubleshooting event</span></span>](intune-troubleshooting-devicemanagementtroubleshootingevent.md)
- [<span data-ttu-id="cb08e-124">デバイスのオペレーティング システムの概要</span><span class="sxs-lookup"><span data-stu-id="cb08e-124">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="cb08e-125">デバイス登録の状態</span><span class="sxs-lookup"><span data-stu-id="cb08e-125">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="cb08e-126">登録のトラブルシューティング イベント</span><span class="sxs-lookup"><span data-stu-id="cb08e-126">Enrollment troubleshooting event</span></span>](intune-troubleshooting-enrollmenttroubleshootingevent.md)
- [<span data-ttu-id="cb08e-127">ローカライズ済み通知メッセージ</span><span class="sxs-lookup"><span data-stu-id="cb08e-127">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="cb08e-128">デバイスの検索アクションの結果</span><span class="sxs-lookup"><span data-stu-id="cb08e-128">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="cb08e-129">管理対象デバイス</span><span class="sxs-lookup"><span data-stu-id="cb08e-129">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="cb08e-130">管理対象デバイスの概要</span><span class="sxs-lookup"><span data-stu-id="cb08e-130">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="cb08e-131">デバイス所有者の種類を管理</span><span class="sxs-lookup"><span data-stu-id="cb08e-131">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="cb08e-132">管理対象デバイスのパートナーは、正常性状態を報告</span><span class="sxs-lookup"><span data-stu-id="cb08e-132">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="cb08e-133">管理エージェントの種類</span><span class="sxs-lookup"><span data-stu-id="cb08e-133">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="cb08e-134">通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="cb08e-134">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="cb08e-135">通知テンプレートのオプションをブランド化</span><span class="sxs-lookup"><span data-stu-id="cb08e-135">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="cb08e-136">リモート アシスタンスの採用状況</span><span class="sxs-lookup"><span data-stu-id="cb08e-136">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="cb08e-137">リモート アシスタンス パートナー</span><span class="sxs-lookup"><span data-stu-id="cb08e-137">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="cb08e-138">リモート ロック アクションの結果</span><span class="sxs-lookup"><span data-stu-id="cb08e-138">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="cb08e-139">パスコードのリセット アクションの結果</span><span class="sxs-lookup"><span data-stu-id="cb08e-139">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="cb08e-140">Windows のデバイス アカウントのアクション パラメーターの更新</span><span class="sxs-lookup"><span data-stu-id="cb08e-140">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="cb08e-141">Windows Defender のスキャン アクションの結果</span><span class="sxs-lookup"><span data-stu-id="cb08e-141">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="cb08e-142">Windows のデバイス アカウント</span><span class="sxs-lookup"><span data-stu-id="cb08e-142">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="cb08e-143">Windows のデバイス AD アカウント</span><span class="sxs-lookup"><span data-stu-id="cb08e-143">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="cb08e-144">Windows のデバイス Azure AD アカウント</span><span class="sxs-lookup"><span data-stu-id="cb08e-144">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)
