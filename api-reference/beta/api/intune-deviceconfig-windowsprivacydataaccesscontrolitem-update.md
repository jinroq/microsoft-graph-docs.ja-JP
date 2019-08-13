---
title: WindowsPrivacyDataAccessControlItem の更新
description: WindowsPrivacyDataAccessControlItem オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4a0565625571c40bb10c800cd428f0986562cbee
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36313735"
---
# <a name="update-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="eb716-103">WindowsPrivacyDataAccessControlItem の更新</span><span class="sxs-lookup"><span data-stu-id="eb716-103">Update windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="eb716-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb716-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb716-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eb716-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb716-106">[WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="eb716-106">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb716-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="eb716-107">Prerequisites</span></span>
<span data-ttu-id="eb716-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eb716-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb716-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eb716-110">Permission type</span></span>|<span data-ttu-id="eb716-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="eb716-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb716-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eb716-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb716-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb716-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eb716-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eb716-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb716-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb716-115">Not supported.</span></span>|
|<span data-ttu-id="eb716-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eb716-116">Application</span></span>|<span data-ttu-id="eb716-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb716-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb716-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eb716-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="request-headers"></a><span data-ttu-id="eb716-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eb716-119">Request headers</span></span>
|<span data-ttu-id="eb716-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eb716-120">Header</span></span>|<span data-ttu-id="eb716-121">値</span><span class="sxs-lookup"><span data-stu-id="eb716-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb716-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb716-122">Authorization</span></span>|<span data-ttu-id="eb716-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="eb716-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb716-124">承諾</span><span class="sxs-lookup"><span data-stu-id="eb716-124">Accept</span></span>|<span data-ttu-id="eb716-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb716-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb716-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="eb716-126">Request body</span></span>
<span data-ttu-id="eb716-127">要求本文で、 [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="eb716-127">In the request body, supply a JSON representation for the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

<span data-ttu-id="eb716-128">次の表に、 [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="eb716-128">The following table shows the properties that are required when you create the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>

|<span data-ttu-id="eb716-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb716-129">Property</span></span>|<span data-ttu-id="eb716-130">型</span><span class="sxs-lookup"><span data-stu-id="eb716-130">Type</span></span>|<span data-ttu-id="eb716-131">説明</span><span class="sxs-lookup"><span data-stu-id="eb716-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb716-132">id</span><span class="sxs-lookup"><span data-stu-id="eb716-132">id</span></span>|<span data-ttu-id="eb716-133">文字列</span><span class="sxs-lookup"><span data-stu-id="eb716-133">String</span></span>|<span data-ttu-id="eb716-134">WindowsPrivacyDataAccessControlItem のキー。</span><span class="sxs-lookup"><span data-stu-id="eb716-134">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="eb716-135">accessLevel</span><span class="sxs-lookup"><span data-stu-id="eb716-135">accessLevel</span></span>|[<span data-ttu-id="eb716-136">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="eb716-136">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="eb716-137">これは、指定されたアプリケーションに割り当てられるプライバシーデータカテゴリのアクセスレベルを示します。</span><span class="sxs-lookup"><span data-stu-id="eb716-137">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="eb716-138">使用可能な値は、`notConfigured`、`forceAllow`、`forceDeny`、`userInControl` です。</span><span class="sxs-lookup"><span data-stu-id="eb716-138">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="eb716-139">引数 datacategory</span><span class="sxs-lookup"><span data-stu-id="eb716-139">dataCategory</span></span>|[<span data-ttu-id="eb716-140">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="eb716-140">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="eb716-141">これは、特定のアクセス制御が適用されるプライバシーデータカテゴリを示します。</span><span class="sxs-lookup"><span data-stu-id="eb716-141">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="eb716-142">可能な値: `notConfigured`、 `accountInfo` `appsRunInBackground` `calendar` `callHistory` `camera` `contacts` `diagnosticsInfo` `email` `location` `messaging` `microphone`、、、、、、、、、、、、 `motion` `notifications` `phone` `radios` `tasks` `syncWithDevices` `trustedDevices`.</span><span class="sxs-lookup"><span data-stu-id="eb716-142">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="eb716-143">App・パッケージ Efamilyname</span><span class="sxs-lookup"><span data-stu-id="eb716-143">appPackageFamilyName</span></span>|<span data-ttu-id="eb716-144">String</span><span class="sxs-lookup"><span data-stu-id="eb716-144">String</span></span>|<span data-ttu-id="eb716-145">Windows アプリのパッケージファミリ名。</span><span class="sxs-lookup"><span data-stu-id="eb716-145">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="eb716-146">設定すると、指定したアプリケーションにアクセスレベルが適用されます。</span><span class="sxs-lookup"><span data-stu-id="eb716-146">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="eb716-147">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="eb716-147">appDisplayName</span></span>|<span data-ttu-id="eb716-148">String</span><span class="sxs-lookup"><span data-stu-id="eb716-148">String</span></span>|<span data-ttu-id="eb716-149">Windows アプリのパッケージファミリ名。</span><span class="sxs-lookup"><span data-stu-id="eb716-149">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="eb716-150">設定すると、指定したアプリケーションにアクセスレベルが適用されます。</span><span class="sxs-lookup"><span data-stu-id="eb716-150">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="eb716-151">応答</span><span class="sxs-lookup"><span data-stu-id="eb716-151">Response</span></span>
<span data-ttu-id="eb716-152">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="eb716-152">If successful, this method returns a `200 OK` response code and an updated [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb716-153">例</span><span class="sxs-lookup"><span data-stu-id="eb716-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb716-154">要求</span><span class="sxs-lookup"><span data-stu-id="eb716-154">Request</span></span>
<span data-ttu-id="eb716-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eb716-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
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

### <a name="response"></a><span data-ttu-id="eb716-156">応答</span><span class="sxs-lookup"><span data-stu-id="eb716-156">Response</span></span>
<span data-ttu-id="eb716-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="eb716-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






