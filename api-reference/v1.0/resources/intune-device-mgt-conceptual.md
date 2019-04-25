---
title: Microsoft Intune でのデバイス管理
description: ''
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4c8f6676647405e8186e9d27466266f6690e2cd1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575234"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="c00c9-102">Microsoft Intune でのデバイス管理</span><span class="sxs-lookup"><span data-stu-id="c00c9-102">Device management in Microsoft Intune</span></span>

> <span data-ttu-id="c00c9-103">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c00c9-103">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="c00c9-104">アクションの状態</span><span class="sxs-lookup"><span data-stu-id="c00c9-104">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="c00c9-105">Apple プッシュ通知証明書</span><span class="sxs-lookup"><span data-stu-id="c00c9-105">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="c00c9-106">監査アクター</span><span class="sxs-lookup"><span data-stu-id="c00c9-106">Audit actor</span></span>](intune-auditing-auditactor.md)
- [<span data-ttu-id="c00c9-107">監査イベント</span><span class="sxs-lookup"><span data-stu-id="c00c9-107">Audit event</span></span>](intune-auditing-auditevent.md)
- [<span data-ttu-id="c00c9-108">監査のプロパティ</span><span class="sxs-lookup"><span data-stu-id="c00c9-108">Audit property</span></span>](intune-auditing-auditproperty.md)
- [<span data-ttu-id="c00c9-109">監査のリソース</span><span class="sxs-lookup"><span data-stu-id="c00c9-109">Audit resource</span></span>](intune-auditing-auditresource.md)
- [<span data-ttu-id="c00c9-110">コンプライアンスのステータス</span><span class="sxs-lookup"><span data-stu-id="c00c9-110">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="c00c9-111">構成マネージャーのクライアントに対応した機能</span><span class="sxs-lookup"><span data-stu-id="c00c9-111">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="c00c9-112">共有の Apple デバイスのアクションの結果からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="c00c9-112">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="c00c9-113">検出されたアプリ</span><span class="sxs-lookup"><span data-stu-id="c00c9-113">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="c00c9-114">デバイスのアクションの結果</span><span class="sxs-lookup"><span data-stu-id="c00c9-114">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="c00c9-115">デバイスの登録失敗の理由</span><span class="sxs-lookup"><span data-stu-id="c00c9-115">Device enrollment failure reason</span></span>](intune-troubleshooting-deviceenrollmentfailurereason.md)
- [<span data-ttu-id="c00c9-116">デバイスの Exchange アクセス状態の要約</span><span class="sxs-lookup"><span data-stu-id="c00c9-116">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="c00c9-117">デバイスの位置情報</span><span class="sxs-lookup"><span data-stu-id="c00c9-117">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="c00c9-118">デバイスの正常性構成証明の状態</span><span class="sxs-lookup"><span data-stu-id="c00c9-118">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="c00c9-119">デバイスの管理 Exchange アクセス状態</span><span class="sxs-lookup"><span data-stu-id="c00c9-119">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="c00c9-120">デバイスの管理 Exchange アクセス状態理由</span><span class="sxs-lookup"><span data-stu-id="c00c9-120">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="c00c9-121">デバイス管理サブスクリプションの状態</span><span class="sxs-lookup"><span data-stu-id="c00c9-121">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="c00c9-122">デバイス管理のトラブルシューティング イベント</span><span class="sxs-lookup"><span data-stu-id="c00c9-122">Device management troubleshooting event</span></span>](intune-troubleshooting-devicemanagementtroubleshootingevent.md)
- [<span data-ttu-id="c00c9-123">デバイスのオペレーティング システムの概要</span><span class="sxs-lookup"><span data-stu-id="c00c9-123">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="c00c9-124">デバイスの登録状態</span><span class="sxs-lookup"><span data-stu-id="c00c9-124">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="c00c9-125">登録のトラブルシューティング イベント</span><span class="sxs-lookup"><span data-stu-id="c00c9-125">Enrollment troubleshooting event</span></span>](intune-troubleshooting-enrollmenttroubleshootingevent.md)
- [<span data-ttu-id="c00c9-126">ローカライズ済み通知メッセージ</span><span class="sxs-lookup"><span data-stu-id="c00c9-126">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="c00c9-127">デバイスの検索アクションの結果</span><span class="sxs-lookup"><span data-stu-id="c00c9-127">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="c00c9-128">管理対象デバイス</span><span class="sxs-lookup"><span data-stu-id="c00c9-128">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="c00c9-129">管理対象デバイスの概要</span><span class="sxs-lookup"><span data-stu-id="c00c9-129">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="c00c9-130">管理対象デバイスの所有者の種類</span><span class="sxs-lookup"><span data-stu-id="c00c9-130">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="c00c9-131">管理対象デバイスのパートナー正常性状態の報告</span><span class="sxs-lookup"><span data-stu-id="c00c9-131">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="c00c9-132">管理エージェントのタイプ</span><span class="sxs-lookup"><span data-stu-id="c00c9-132">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="c00c9-133">通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="c00c9-133">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="c00c9-134">通知テンプレートのブランド化オプション</span><span class="sxs-lookup"><span data-stu-id="c00c9-134">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="c00c9-135">リモート アシスタンス オンボード状態</span><span class="sxs-lookup"><span data-stu-id="c00c9-135">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="c00c9-136">リモート アシスタンス パートナー</span><span class="sxs-lookup"><span data-stu-id="c00c9-136">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="c00c9-137">リモート ロック アクションの結果</span><span class="sxs-lookup"><span data-stu-id="c00c9-137">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="c00c9-138">パスコードのリセット アクションの結果</span><span class="sxs-lookup"><span data-stu-id="c00c9-138">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="c00c9-139">Windows のデバイス アカウントのアクション パラメーターの更新</span><span class="sxs-lookup"><span data-stu-id="c00c9-139">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="c00c9-140">Windows Defender のスキャン アクションの結果</span><span class="sxs-lookup"><span data-stu-id="c00c9-140">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="c00c9-141">Windows のデバイス アカウント</span><span class="sxs-lookup"><span data-stu-id="c00c9-141">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="c00c9-142">Windows のデバイス AD アカウント</span><span class="sxs-lookup"><span data-stu-id="c00c9-142">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="c00c9-143">Windows のデバイス Azure AD アカウント</span><span class="sxs-lookup"><span data-stu-id="c00c9-143">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)
