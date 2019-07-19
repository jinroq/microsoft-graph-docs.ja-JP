---
title: WindowsPrivacyDataAccessControlItem の更新
description: WindowsPrivacyDataAccessControlItem オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3208d5f4eb7ac1fe20ea3d280f8522358ba8867
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961379"
---
# <a name="update-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="05dfb-103">WindowsPrivacyDataAccessControlItem の更新</span><span class="sxs-lookup"><span data-stu-id="05dfb-103">Update windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="05dfb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05dfb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05dfb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="05dfb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05dfb-106">[WindowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="05dfb-106">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05dfb-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="05dfb-107">Prerequisites</span></span>
<span data-ttu-id="05dfb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="05dfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05dfb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="05dfb-110">Permission type</span></span>|<span data-ttu-id="05dfb-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="05dfb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05dfb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="05dfb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="05dfb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05dfb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="05dfb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="05dfb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05dfb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05dfb-115">Not supported.</span></span>|
|<span data-ttu-id="05dfb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="05dfb-116">Application</span></span>|<span data-ttu-id="05dfb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05dfb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05dfb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="05dfb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="request-headers"></a><span data-ttu-id="05dfb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="05dfb-119">Request headers</span></span>
|<span data-ttu-id="05dfb-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="05dfb-120">Header</span></span>|<span data-ttu-id="05dfb-121">値</span><span class="sxs-lookup"><span data-stu-id="05dfb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05dfb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="05dfb-122">Authorization</span></span>|<span data-ttu-id="05dfb-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="05dfb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05dfb-124">承諾</span><span class="sxs-lookup"><span data-stu-id="05dfb-124">Accept</span></span>|<span data-ttu-id="05dfb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="05dfb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05dfb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="05dfb-126">Request body</span></span>
<span data-ttu-id="05dfb-127">要求本文で、 [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="05dfb-127">In the request body, supply a JSON representation for the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

<span data-ttu-id="05dfb-128">次の表に、 [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="05dfb-128">The following table shows the properties that are required when you create the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>

|<span data-ttu-id="05dfb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05dfb-129">Property</span></span>|<span data-ttu-id="05dfb-130">型</span><span class="sxs-lookup"><span data-stu-id="05dfb-130">Type</span></span>|<span data-ttu-id="05dfb-131">説明</span><span class="sxs-lookup"><span data-stu-id="05dfb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05dfb-132">id</span><span class="sxs-lookup"><span data-stu-id="05dfb-132">id</span></span>|<span data-ttu-id="05dfb-133">文字列</span><span class="sxs-lookup"><span data-stu-id="05dfb-133">String</span></span>|<span data-ttu-id="05dfb-134">WindowsPrivacyDataAccessControlItem のキー。</span><span class="sxs-lookup"><span data-stu-id="05dfb-134">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="05dfb-135">accessLevel</span><span class="sxs-lookup"><span data-stu-id="05dfb-135">accessLevel</span></span>|[<span data-ttu-id="05dfb-136">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="05dfb-136">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="05dfb-137">これは、指定されたアプリケーションに割り当てられるプライバシーデータカテゴリのアクセスレベルを示します。</span><span class="sxs-lookup"><span data-stu-id="05dfb-137">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="05dfb-138">使用可能な値は、`notConfigured`、`forceAllow`、`forceDeny`、`userInControl` です。</span><span class="sxs-lookup"><span data-stu-id="05dfb-138">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="05dfb-139">引数 datacategory</span><span class="sxs-lookup"><span data-stu-id="05dfb-139">dataCategory</span></span>|[<span data-ttu-id="05dfb-140">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="05dfb-140">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="05dfb-141">これは、特定のアクセス制御が適用されるプライバシーデータカテゴリを示します。</span><span class="sxs-lookup"><span data-stu-id="05dfb-141">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="05dfb-142">可能な値: `notConfigured`、 `accountInfo` `appsRunInBackground` `calendar` `callHistory` `camera` `contacts` `diagnosticsInfo` `email` `location` `messaging` `microphone`、、、、、、、、、、、、 `motion` `notifications` `phone` `radios` `tasks` `syncWithDevices` `trustedDevices`.</span><span class="sxs-lookup"><span data-stu-id="05dfb-142">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="05dfb-143">App・パッケージ Efamilyname</span><span class="sxs-lookup"><span data-stu-id="05dfb-143">appPackageFamilyName</span></span>|<span data-ttu-id="05dfb-144">String</span><span class="sxs-lookup"><span data-stu-id="05dfb-144">String</span></span>|<span data-ttu-id="05dfb-145">Windows アプリのパッケージファミリ名。</span><span class="sxs-lookup"><span data-stu-id="05dfb-145">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="05dfb-146">設定すると、指定したアプリケーションにアクセスレベルが適用されます。</span><span class="sxs-lookup"><span data-stu-id="05dfb-146">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="05dfb-147">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="05dfb-147">appDisplayName</span></span>|<span data-ttu-id="05dfb-148">String</span><span class="sxs-lookup"><span data-stu-id="05dfb-148">String</span></span>|<span data-ttu-id="05dfb-149">Windows アプリのパッケージファミリ名。</span><span class="sxs-lookup"><span data-stu-id="05dfb-149">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="05dfb-150">設定すると、指定したアプリケーションにアクセスレベルが適用されます。</span><span class="sxs-lookup"><span data-stu-id="05dfb-150">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="05dfb-151">応答</span><span class="sxs-lookup"><span data-stu-id="05dfb-151">Response</span></span>
<span data-ttu-id="05dfb-152">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="05dfb-152">If successful, this method returns a `200 OK` response code and an updated [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05dfb-153">例</span><span class="sxs-lookup"><span data-stu-id="05dfb-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="05dfb-154">要求</span><span class="sxs-lookup"><span data-stu-id="05dfb-154">Request</span></span>
<span data-ttu-id="05dfb-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="05dfb-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="05dfb-156">応答</span><span class="sxs-lookup"><span data-stu-id="05dfb-156">Response</span></span>
<span data-ttu-id="05dfb-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="05dfb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





