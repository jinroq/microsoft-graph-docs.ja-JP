---
title: Microsoft Intune を使用してアプリを管理する
description: '次の Graph リソースを使用して、Intune でモバイル アプリを管理できます。  '
author: tfitzmac
ms.openlocfilehash: cd0a9f391fc3d795b8599bd9e97847345908477f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332194"
---
# <a name="manage-apps-using-microsoft-intune"></a><span data-ttu-id="5cbba-103">Microsoft Intune を使用してアプリを管理する</span><span class="sxs-lookup"><span data-stu-id="5cbba-103">Manage apps using Microsoft Intune</span></span>

> <span data-ttu-id="5cbba-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5cbba-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="5cbba-105">次の Graph リソースを使用して、Intune でモバイル アプリを管理できます。</span><span class="sxs-lookup"><span data-stu-id="5cbba-105">The following Graph resources are available to manage mobile apps in Intune:</span></span>  

- [<span data-ttu-id="5cbba-106">Android LOB アプリ</span><span class="sxs-lookup"><span data-stu-id="5cbba-106">Android LOB app</span></span>](intune-apps-androidlobapp.md)
- [<span data-ttu-id="5cbba-107">最小構成の Android オペレーティング システム</span><span class="sxs-lookup"><span data-stu-id="5cbba-107">Android minimum operating system</span></span>](intune-apps-androidminimumoperatingsystem.md)
- [<span data-ttu-id="5cbba-108">Android ストア アプリ</span><span class="sxs-lookup"><span data-stu-id="5cbba-108">Android store app</span></span>](intune-apps-androidstoreapp.md)
- [<span data-ttu-id="5cbba-109">アプリケーション構成の設定項目</span><span class="sxs-lookup"><span data-stu-id="5cbba-109">App configuration setting item</span></span>](intune-apps-appconfigurationsettingitem.md)
- [<span data-ttu-id="5cbba-110">デバイスのインストール状態</span><span class="sxs-lookup"><span data-stu-id="5cbba-110">Device install state</span></span>](intune-books-deviceinstallstate.md)
- [<span data-ttu-id="5cbba-111">電子書籍のインストールの概要</span><span class="sxs-lookup"><span data-stu-id="5cbba-111">E-book install summary</span></span>](intune-books-ebookinstallsummary.md)
- [<span data-ttu-id="5cbba-112">ファイル暗号化情報</span><span class="sxs-lookup"><span data-stu-id="5cbba-112">File encryption info</span></span>](intune-apps-fileencryptioninfo.md)
- [<span data-ttu-id="5cbba-113">インストール状態</span><span class="sxs-lookup"><span data-stu-id="5cbba-113">Install state</span></span>](intune-books-installstate.md)
- [<span data-ttu-id="5cbba-114">iOS デバイスの種類</span><span class="sxs-lookup"><span data-stu-id="5cbba-114">iOS device type</span></span>](intune-apps-iosdevicetype.md)
- [<span data-ttu-id="5cbba-115">iOS LOB アプリ</span><span class="sxs-lookup"><span data-stu-id="5cbba-115">iOS LOB app</span></span>](intune-apps-ioslobapp.md)
- [<span data-ttu-id="5cbba-116">iOS LOB アプリの割り当ての設定</span><span class="sxs-lookup"><span data-stu-id="5cbba-116">iOS LOB app assignment settings</span></span>](intune-apps-ioslobappassignmentsettings.md)
- [<span data-ttu-id="5cbba-117">最小構成の iOS オペレーティング システム</span><span class="sxs-lookup"><span data-stu-id="5cbba-117">iOS minimum operating system</span></span>](intune-apps-iosminimumoperatingsystem.md)
- [<span data-ttu-id="5cbba-118">iOS モバイル アプリケーションの構成</span><span class="sxs-lookup"><span data-stu-id="5cbba-118">iOS mobile app configuration</span></span>](intune-apps-iosmobileappconfiguration.md)
- [<span data-ttu-id="5cbba-119">iOS ストア アプリ</span><span class="sxs-lookup"><span data-stu-id="5cbba-119">iOS store app</span></span>](intune-apps-iosstoreapp.md)
- [<span data-ttu-id="5cbba-120">iOS ストア アプリの割り当ての設定</span><span class="sxs-lookup"><span data-stu-id="5cbba-120">iOS store app assignment settings</span></span>](intune-apps-iosstoreappassignmentsettings.md)
- [<span data-ttu-id="5cbba-121">iOS VPP アプリ</span><span class="sxs-lookup"><span data-stu-id="5cbba-121">iOS VPP app</span></span>](intune-apps-iosvppapp.md)
- [<span data-ttu-id="5cbba-122">iOS VPP アプリの割り当ての設定</span><span class="sxs-lookup"><span data-stu-id="5cbba-122">iOS VPP app assignment settings</span></span>](intune-apps-iosvppappassignmentsettings.md)
- [<span data-ttu-id="5cbba-123">iOS VPP の電子書籍</span><span class="sxs-lookup"><span data-stu-id="5cbba-123">iOS VPP e-book</span></span>](intune-books-iosvppebook.md)
- [<span data-ttu-id="5cbba-124">iOS VPP 電子書籍の割り当て</span><span class="sxs-lookup"><span data-stu-id="5cbba-124">iOS VPP e-book assignment</span></span>](intune-books-iosvppebookassignment.md)
- [<span data-ttu-id="5cbba-125">macOS Office スイート アプリ</span><span class="sxs-lookup"><span data-stu-id="5cbba-125">macOS office suite app</span></span>](intune-apps-macosofficesuiteapp.md)
- [<span data-ttu-id="5cbba-126">管理対象 Android LOB アプリ</span><span class="sxs-lookup"><span data-stu-id="5cbba-126">Managed android LOB app</span></span>](intune-apps-managedandroidlobapp.md)
- [<span data-ttu-id="5cbba-127">管理対象 Android ストア アプリ</span><span class="sxs-lookup"><span data-stu-id="5cbba-127">Managed android store app</span></span>](intune-apps-managedandroidstoreapp.md)
- [<span data-ttu-id="5cbba-128">管理対象アプリ</span><span class="sxs-lookup"><span data-stu-id="5cbba-128">Managed app</span></span>](intune-apps-managedapp.md)
- [<span data-ttu-id="5cbba-129">マネージ アプリケーションの可用性</span><span class="sxs-lookup"><span data-stu-id="5cbba-129">Managed app availability</span></span>](intune-apps-managedappavailability.md)
- [<span data-ttu-id="5cbba-130">管理対象デバイスのモバイル アプリ構成</span><span class="sxs-lookup"><span data-stu-id="5cbba-130">Managed device mobile app configuration</span></span>](intune-apps-manageddevicemobileappconfiguration.md)
- [<span data-ttu-id="5cbba-131">管理対象デバイスのモバイル アプリ構成の割り当て</span><span class="sxs-lookup"><span data-stu-id="5cbba-131">Managed device mobile app configuration assignment</span></span>](intune-apps-manageddevicemobileappconfigurationassignment.md)
- [<span data-ttu-id="5cbba-132">デバイスのモバイル アプリケーションの構成デバイスの状態を管理</span><span class="sxs-lookup"><span data-stu-id="5cbba-132">Managed device mobile app configuration device status</span></span>](intune-apps-manageddevicemobileappconfigurationdevicestatus.md)
- [<span data-ttu-id="5cbba-133">管理対象デバイスのモバイル アプリ構成のデバイスの要約</span><span class="sxs-lookup"><span data-stu-id="5cbba-133">Managed device mobile app configuration device summary</span></span>](intune-apps-manageddevicemobileappconfigurationdevicesummary.md)
- [<span data-ttu-id="5cbba-134">管理対象デバイスのモバイル アプリ構成のユーザー状態</span><span class="sxs-lookup"><span data-stu-id="5cbba-134">Managed device mobile app configuration user status</span></span>](intune-apps-manageddevicemobileappconfigurationuserstatus.md)
- [<span data-ttu-id="5cbba-135">管理対象デバイスのモバイル アプリ構成のユーザー要約</span><span class="sxs-lookup"><span data-stu-id="5cbba-135">Managed device mobile app configuration user summary</span></span>](intune-apps-manageddevicemobileappconfigurationusersummary.md)
- [<span data-ttu-id="5cbba-136">管理対象の電子書籍</span><span class="sxs-lookup"><span data-stu-id="5cbba-136">Managed e-book</span></span>](intune-books-managedebook.md)
- [<span data-ttu-id="5cbba-137">管理対象電子書籍の割り当て</span><span class="sxs-lookup"><span data-stu-id="5cbba-137">Managed e-book assignment</span></span>](intune-books-managedebookassignment.md)
- [<span data-ttu-id="5cbba-138">管理対象 iOS LOB アプリ</span><span class="sxs-lookup"><span data-stu-id="5cbba-138">Managed iOS LOB app</span></span>](intune-apps-managedioslobapp.md)
- [<span data-ttu-id="5cbba-139">管理対象 iOS ストア アプリ</span><span class="sxs-lookup"><span data-stu-id="5cbba-139">Managed iOS store app</span></span>](intune-apps-managediosstoreapp.md)
- [<span data-ttu-id="5cbba-140">管理対象モバイル LOB アプリ</span><span class="sxs-lookup"><span data-stu-id="5cbba-140">Managed mobile LOB app</span></span>](intune-apps-managedmobilelobapp.md)
- [<span data-ttu-id="5cbba-141">MDM アプリケーション設定のキーの種類</span><span class="sxs-lookup"><span data-stu-id="5cbba-141">MDM app config key type</span></span>](intune-apps-mdmappconfigkeytype.md)
- [<span data-ttu-id="5cbba-142">ビジネス向け Microsoft Store のアプリ</span><span class="sxs-lookup"><span data-stu-id="5cbba-142">Microsoft store for business app</span></span>](intune-apps-microsoftstoreforbusinessapp.md)
- [<span data-ttu-id="5cbba-143">ビジネス向け Microsoft Store のアプリの割り当ての設定</span><span class="sxs-lookup"><span data-stu-id="5cbba-143">Microsoft store for business app assignment settings</span></span>](intune-apps-microsoftstoreforbusinessappassignmentsettings.md)
- [<span data-ttu-id="5cbba-144">マイクロソフトは、ビジネス ライセンスの種類を保存します。</span><span class="sxs-lookup"><span data-stu-id="5cbba-144">Microsoft store for business license type</span></span>](intune-apps-microsoftstoreforbusinesslicensetype.md)
- [<span data-ttu-id="5cbba-145">モバイル アプリ</span><span class="sxs-lookup"><span data-stu-id="5cbba-145">Mobile app</span></span>](intune-apps-mobileapp.md)
- [<span data-ttu-id="5cbba-146">モバイル アプリの割り当て</span><span class="sxs-lookup"><span data-stu-id="5cbba-146">Mobile app assignment</span></span>](intune-apps-mobileappassignment.md)
- [<span data-ttu-id="5cbba-147">モバイル アプリの割り当ての設定</span><span class="sxs-lookup"><span data-stu-id="5cbba-147">Mobile app assignment settings</span></span>](intune-apps-mobileappassignmentsettings.md)
- [<span data-ttu-id="5cbba-148">モバイル アプリのカテゴリ</span><span class="sxs-lookup"><span data-stu-id="5cbba-148">Mobile app category</span></span>](intune-apps-mobileappcategory.md)
- [<span data-ttu-id="5cbba-149">モバイル アプリ コンテンツ</span><span class="sxs-lookup"><span data-stu-id="5cbba-149">Mobile app content</span></span>](intune-apps-mobileappcontent.md)
- [<span data-ttu-id="5cbba-150">モバイル アプリ コンテンツ ファイル</span><span class="sxs-lookup"><span data-stu-id="5cbba-150">Mobile app content file</span></span>](intune-apps-mobileappcontentfile.md)
- [<span data-ttu-id="5cbba-151">モバイル アプリケーション コンテンツ ファイルのアップロードの状態</span><span class="sxs-lookup"><span data-stu-id="5cbba-151">Mobile app content file upload state</span></span>](intune-apps-mobileappcontentfileuploadstate.md)
- [<span data-ttu-id="5cbba-152">モバイル アプリケーションの公開状況</span><span class="sxs-lookup"><span data-stu-id="5cbba-152">Mobile app publishing state</span></span>](intune-apps-mobileapppublishingstate.md)
- [<span data-ttu-id="5cbba-153">モバイル LOB アプリ</span><span class="sxs-lookup"><span data-stu-id="5cbba-153">Mobile LOB app</span></span>](intune-apps-mobilelobapp.md)
- [<span data-ttu-id="5cbba-154">ユーザーのインストール状態の概要</span><span class="sxs-lookup"><span data-stu-id="5cbba-154">User install state summary</span></span>](intune-books-userinstallstatesummary.md)
- [<span data-ttu-id="5cbba-155">VPP ライセンスの種類</span><span class="sxs-lookup"><span data-stu-id="5cbba-155">VPP licensing type</span></span>](intune-apps-vpplicensingtype.md)
- [<span data-ttu-id="5cbba-156">Web アプリ</span><span class="sxs-lookup"><span data-stu-id="5cbba-156">Web app</span></span>](intune-apps-webapp.md)
- [<span data-ttu-id="5cbba-157">Windows のアーキテクチャ</span><span class="sxs-lookup"><span data-stu-id="5cbba-157">Windows architecture</span></span>](intune-apps-windowsarchitecture.md)
- [<span data-ttu-id="5cbba-158">Windows デバイスの種類</span><span class="sxs-lookup"><span data-stu-id="5cbba-158">Windows device type</span></span>](intune-apps-windowsdevicetype.md)
- [<span data-ttu-id="5cbba-159">最小構成の Windows オペレーティング システム</span><span class="sxs-lookup"><span data-stu-id="5cbba-159">Windows minimum operating system</span></span>](intune-apps-windowsminimumoperatingsystem.md)
- [<span data-ttu-id="5cbba-160">Windows Mobile MSI</span><span class="sxs-lookup"><span data-stu-id="5cbba-160">Windows mobile MSI</span></span>](intune-apps-windowsmobilemsi.md)
- [<span data-ttu-id="5cbba-161">Windows ユニバーサル AppX</span><span class="sxs-lookup"><span data-stu-id="5cbba-161">Windows universal AppX</span></span>](intune-apps-windowsuniversalappx.md)