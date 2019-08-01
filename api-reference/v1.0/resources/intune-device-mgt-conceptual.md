---
title: Microsoft Intune でのデバイス管理
description: Microsoft Intune のデバイス管理リソース
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 476ae4d03fae4653a1465952074f521d6df1123c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031977"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="ee9fb-103">Microsoft Intune でのデバイス管理</span><span class="sxs-lookup"><span data-stu-id="ee9fb-103">Device management in Microsoft Intune</span></span>

> <span data-ttu-id="ee9fb-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ee9fb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="ee9fb-105">アクションの状態</span><span class="sxs-lookup"><span data-stu-id="ee9fb-105">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="ee9fb-106">Apple プッシュ通知証明書</span><span class="sxs-lookup"><span data-stu-id="ee9fb-106">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="ee9fb-107">監査アクター</span><span class="sxs-lookup"><span data-stu-id="ee9fb-107">Audit actor</span></span>](intune-auditing-auditactor.md)
- [<span data-ttu-id="ee9fb-108">監査イベント</span><span class="sxs-lookup"><span data-stu-id="ee9fb-108">Audit event</span></span>](intune-auditing-auditevent.md)
- [<span data-ttu-id="ee9fb-109">監査のプロパティ</span><span class="sxs-lookup"><span data-stu-id="ee9fb-109">Audit property</span></span>](intune-auditing-auditproperty.md)
- [<span data-ttu-id="ee9fb-110">監査のリソース</span><span class="sxs-lookup"><span data-stu-id="ee9fb-110">Audit resource</span></span>](intune-auditing-auditresource.md)
- [<span data-ttu-id="ee9fb-111">コンプライアンスのステータス</span><span class="sxs-lookup"><span data-stu-id="ee9fb-111">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="ee9fb-112">構成マネージャーのクライアントに対応した機能</span><span class="sxs-lookup"><span data-stu-id="ee9fb-112">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="ee9fb-113">共有の Apple デバイスのアクションの結果からユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="ee9fb-113">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="ee9fb-114">検出されたアプリ</span><span class="sxs-lookup"><span data-stu-id="ee9fb-114">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="ee9fb-115">デバイスのアクションの結果</span><span class="sxs-lookup"><span data-stu-id="ee9fb-115">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="ee9fb-116">デバイスの登録失敗の理由</span><span class="sxs-lookup"><span data-stu-id="ee9fb-116">Device enrollment failure reason</span></span>](intune-troubleshooting-deviceenrollmentfailurereason.md)
- [<span data-ttu-id="ee9fb-117">デバイスの Exchange アクセス状態の要約</span><span class="sxs-lookup"><span data-stu-id="ee9fb-117">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="ee9fb-118">デバイスの位置情報</span><span class="sxs-lookup"><span data-stu-id="ee9fb-118">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="ee9fb-119">デバイスの正常性構成証明の状態</span><span class="sxs-lookup"><span data-stu-id="ee9fb-119">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="ee9fb-120">デバイスの管理 Exchange アクセス状態</span><span class="sxs-lookup"><span data-stu-id="ee9fb-120">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="ee9fb-121">デバイスの管理 Exchange アクセス状態理由</span><span class="sxs-lookup"><span data-stu-id="ee9fb-121">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="ee9fb-122">デバイス管理サブスクリプションの状態</span><span class="sxs-lookup"><span data-stu-id="ee9fb-122">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="ee9fb-123">デバイス管理のトラブルシューティング イベント</span><span class="sxs-lookup"><span data-stu-id="ee9fb-123">Device management troubleshooting event</span></span>](intune-troubleshooting-devicemanagementtroubleshootingevent.md)
- [<span data-ttu-id="ee9fb-124">デバイスのオペレーティング システムの概要</span><span class="sxs-lookup"><span data-stu-id="ee9fb-124">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="ee9fb-125">デバイスの登録状態</span><span class="sxs-lookup"><span data-stu-id="ee9fb-125">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="ee9fb-126">登録のトラブルシューティング イベント</span><span class="sxs-lookup"><span data-stu-id="ee9fb-126">Enrollment troubleshooting event</span></span>](intune-troubleshooting-enrollmenttroubleshootingevent.md)
- [<span data-ttu-id="ee9fb-127">ローカライズ済み通知メッセージ</span><span class="sxs-lookup"><span data-stu-id="ee9fb-127">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="ee9fb-128">デバイスの検索アクションの結果</span><span class="sxs-lookup"><span data-stu-id="ee9fb-128">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="ee9fb-129">管理対象デバイス</span><span class="sxs-lookup"><span data-stu-id="ee9fb-129">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="ee9fb-130">管理対象デバイスの概要</span><span class="sxs-lookup"><span data-stu-id="ee9fb-130">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="ee9fb-131">管理対象デバイスの所有者の種類</span><span class="sxs-lookup"><span data-stu-id="ee9fb-131">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="ee9fb-132">管理対象デバイスのパートナー正常性状態の報告</span><span class="sxs-lookup"><span data-stu-id="ee9fb-132">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="ee9fb-133">管理エージェントのタイプ</span><span class="sxs-lookup"><span data-stu-id="ee9fb-133">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="ee9fb-134">通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="ee9fb-134">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="ee9fb-135">通知テンプレートのブランド化オプション</span><span class="sxs-lookup"><span data-stu-id="ee9fb-135">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="ee9fb-136">リモート アシスタンス オンボード状態</span><span class="sxs-lookup"><span data-stu-id="ee9fb-136">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="ee9fb-137">リモート アシスタンス パートナー</span><span class="sxs-lookup"><span data-stu-id="ee9fb-137">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="ee9fb-138">リモート ロック アクションの結果</span><span class="sxs-lookup"><span data-stu-id="ee9fb-138">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="ee9fb-139">パスコードのリセット アクションの結果</span><span class="sxs-lookup"><span data-stu-id="ee9fb-139">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="ee9fb-140">Windows のデバイス アカウントのアクション パラメーターの更新</span><span class="sxs-lookup"><span data-stu-id="ee9fb-140">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="ee9fb-141">Windows Defender のスキャン アクションの結果</span><span class="sxs-lookup"><span data-stu-id="ee9fb-141">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="ee9fb-142">Windows のデバイス アカウント</span><span class="sxs-lookup"><span data-stu-id="ee9fb-142">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="ee9fb-143">Windows のデバイス AD アカウント</span><span class="sxs-lookup"><span data-stu-id="ee9fb-143">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="ee9fb-144">Windows のデバイス Azure AD アカウント</span><span class="sxs-lookup"><span data-stu-id="ee9fb-144">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)
