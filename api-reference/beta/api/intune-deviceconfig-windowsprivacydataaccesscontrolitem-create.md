---
title: windowsPrivacyDataAccessControlItem を作成する
description: 新しい windowsPrivacyDataAccessControlItem オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e4d1be396c9532f7b62ded51aeb095a831af320
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32511929"
---
# <a name="create-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="d78c5-103">windowsPrivacyDataAccessControlItem を作成する</span><span class="sxs-lookup"><span data-stu-id="d78c5-103">Create windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="d78c5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d78c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d78c5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d78c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d78c5-106">新しい[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d78c5-106">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d78c5-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d78c5-107">Prerequisites</span></span>
<span data-ttu-id="d78c5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d78c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d78c5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d78c5-110">Permission type</span></span>|<span data-ttu-id="d78c5-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d78c5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d78c5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d78c5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d78c5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d78c5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d78c5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d78c5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d78c5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d78c5-115">Not supported.</span></span>|
|<span data-ttu-id="d78c5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d78c5-116">Application</span></span>|<span data-ttu-id="d78c5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d78c5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d78c5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d78c5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="d78c5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d78c5-119">Request headers</span></span>
|<span data-ttu-id="d78c5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d78c5-120">Header</span></span>|<span data-ttu-id="d78c5-121">値</span><span class="sxs-lookup"><span data-stu-id="d78c5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d78c5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d78c5-122">Authorization</span></span>|<span data-ttu-id="d78c5-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d78c5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d78c5-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d78c5-124">Accept</span></span>|<span data-ttu-id="d78c5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d78c5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d78c5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d78c5-126">Request body</span></span>
<span data-ttu-id="d78c5-127">要求本文で、windowsPrivacyDataAccessControlItem オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d78c5-127">In the request body, supply a JSON representation for the windowsPrivacyDataAccessControlItem object.</span></span>

<span data-ttu-id="d78c5-128">次の表に、windowsPrivacyDataAccessControlItem の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d78c5-128">The following table shows the properties that are required when you create the windowsPrivacyDataAccessControlItem.</span></span>

|<span data-ttu-id="d78c5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d78c5-129">Property</span></span>|<span data-ttu-id="d78c5-130">型</span><span class="sxs-lookup"><span data-stu-id="d78c5-130">Type</span></span>|<span data-ttu-id="d78c5-131">説明</span><span class="sxs-lookup"><span data-stu-id="d78c5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d78c5-132">id</span><span class="sxs-lookup"><span data-stu-id="d78c5-132">id</span></span>|<span data-ttu-id="d78c5-133">String</span><span class="sxs-lookup"><span data-stu-id="d78c5-133">String</span></span>|<span data-ttu-id="d78c5-134">WindowsPrivacyDataAccessControlItem のキー。</span><span class="sxs-lookup"><span data-stu-id="d78c5-134">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="d78c5-135">accessLevel</span><span class="sxs-lookup"><span data-stu-id="d78c5-135">accessLevel</span></span>|[<span data-ttu-id="d78c5-136">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="d78c5-136">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="d78c5-137">これは、指定されたアプリケーションに割り当てられるプライバシーデータカテゴリのアクセスレベルを示します。</span><span class="sxs-lookup"><span data-stu-id="d78c5-137">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="d78c5-138">可能な値は、`notConfigured`、`forceAllow`、`forceDeny`、`userInControl` です。</span><span class="sxs-lookup"><span data-stu-id="d78c5-138">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="d78c5-139">引数 datacategory</span><span class="sxs-lookup"><span data-stu-id="d78c5-139">dataCategory</span></span>|[<span data-ttu-id="d78c5-140">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="d78c5-140">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="d78c5-141">これは、特定のアクセス制御が適用されるプライバシーデータカテゴリを示します。</span><span class="sxs-lookup"><span data-stu-id="d78c5-141">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="d78c5-142">可能な値: `notConfigured`、 `accountInfo` `appsRunInBackground` `calendar` `callHistory` `camera` `contacts` `diagnosticsInfo` `email` `location` `messaging` `microphone`、、、、、、、、、、、、 `motion` `notifications` `phone` `radios` `tasks` `syncWithDevices` `trustedDevices`.</span><span class="sxs-lookup"><span data-stu-id="d78c5-142">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="d78c5-143">app・パッケージ efamilyname</span><span class="sxs-lookup"><span data-stu-id="d78c5-143">appPackageFamilyName</span></span>|<span data-ttu-id="d78c5-144">String</span><span class="sxs-lookup"><span data-stu-id="d78c5-144">String</span></span>|<span data-ttu-id="d78c5-145">Windows アプリのパッケージファミリ名。</span><span class="sxs-lookup"><span data-stu-id="d78c5-145">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="d78c5-146">設定すると、指定したアプリケーションにアクセスレベルが適用されます。</span><span class="sxs-lookup"><span data-stu-id="d78c5-146">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="d78c5-147">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="d78c5-147">appDisplayName</span></span>|<span data-ttu-id="d78c5-148">String</span><span class="sxs-lookup"><span data-stu-id="d78c5-148">String</span></span>|<span data-ttu-id="d78c5-149">Windows アプリのパッケージファミリ名。</span><span class="sxs-lookup"><span data-stu-id="d78c5-149">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="d78c5-150">設定すると、指定したアプリケーションにアクセスレベルが適用されます。</span><span class="sxs-lookup"><span data-stu-id="d78c5-150">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="d78c5-151">応答</span><span class="sxs-lookup"><span data-stu-id="d78c5-151">Response</span></span>
<span data-ttu-id="d78c5-152">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d78c5-152">If successful, this method returns a `201 Created` response code and a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d78c5-153">例</span><span class="sxs-lookup"><span data-stu-id="d78c5-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="d78c5-154">要求</span><span class="sxs-lookup"><span data-stu-id="d78c5-154">Request</span></span>
<span data-ttu-id="d78c5-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d78c5-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
Content-type: application/json
Content-length: 250

{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "accessLevel": "forceAllow",
  "dataCategory": "accountInfo",
  "appPackageFamilyName": "App Package Family Name value",
  "appDisplayName": "App Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="d78c5-156">応答</span><span class="sxs-lookup"><span data-stu-id="d78c5-156">Response</span></span>
<span data-ttu-id="d78c5-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d78c5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 299

{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "id": "03b15556-5556-03b1-5655-b1035655b103",
  "accessLevel": "forceAllow",
  "dataCategory": "accountInfo",
  "appPackageFamilyName": "App Package Family Name value",
  "appDisplayName": "App Display Name value"
}
```





