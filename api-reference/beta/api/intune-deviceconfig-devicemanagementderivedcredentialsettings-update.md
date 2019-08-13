---
title: DeviceManagementDerivedCredentialSettings の更新
description: DeviceManagementDerivedCredentialSettings オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 007126ea25822a635b946de00def06dbbf459c27
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36339751"
---
# <a name="update-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="4c253-103">DeviceManagementDerivedCredentialSettings の更新</span><span class="sxs-lookup"><span data-stu-id="4c253-103">Update deviceManagementDerivedCredentialSettings</span></span>

> <span data-ttu-id="4c253-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c253-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c253-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c253-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c253-106">[DeviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4c253-106">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c253-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4c253-107">Prerequisites</span></span>
<span data-ttu-id="4c253-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c253-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c253-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c253-110">Permission type</span></span>|<span data-ttu-id="4c253-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4c253-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c253-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4c253-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4c253-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c253-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c253-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c253-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c253-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c253-115">Not supported.</span></span>|
|<span data-ttu-id="4c253-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c253-116">Application</span></span>|<span data-ttu-id="4c253-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c253-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c253-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c253-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosVpnConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosDerivedCredentialAuthenticationConfiguration/derivedCredentialSettings
```

## <a name="request-headers"></a><span data-ttu-id="4c253-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c253-119">Request headers</span></span>
|<span data-ttu-id="4c253-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c253-120">Header</span></span>|<span data-ttu-id="4c253-121">値</span><span class="sxs-lookup"><span data-stu-id="4c253-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c253-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c253-122">Authorization</span></span>|<span data-ttu-id="4c253-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c253-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c253-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4c253-124">Accept</span></span>|<span data-ttu-id="4c253-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c253-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c253-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4c253-126">Request body</span></span>
<span data-ttu-id="4c253-127">要求本文で、 [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4c253-127">In the request body, supply a JSON representation for the [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) object.</span></span>

<span data-ttu-id="4c253-128">次の表に、 [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4c253-128">The following table shows the properties that are required when you create the [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md).</span></span>

|<span data-ttu-id="4c253-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c253-129">Property</span></span>|<span data-ttu-id="4c253-130">型</span><span class="sxs-lookup"><span data-stu-id="4c253-130">Type</span></span>|<span data-ttu-id="4c253-131">説明</span><span class="sxs-lookup"><span data-stu-id="4c253-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c253-132">id</span><span class="sxs-lookup"><span data-stu-id="4c253-132">id</span></span>|<span data-ttu-id="4c253-133">文字列</span><span class="sxs-lookup"><span data-stu-id="4c253-133">String</span></span>|<span data-ttu-id="4c253-134">派生した資格情報の一意識別子</span><span class="sxs-lookup"><span data-stu-id="4c253-134">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="4c253-135">helpUrl</span><span class="sxs-lookup"><span data-stu-id="4c253-135">helpUrl</span></span>|<span data-ttu-id="4c253-136">String</span><span class="sxs-lookup"><span data-stu-id="4c253-136">String</span></span>|<span data-ttu-id="4c253-137">エンドユーザーが会社のポータルを使用して派生した資格情報を取得するときに、エンドユーザーがアクセスできる URL。</span><span class="sxs-lookup"><span data-stu-id="4c253-137">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="4c253-138">displayName</span><span class="sxs-lookup"><span data-stu-id="4c253-138">displayName</span></span>|<span data-ttu-id="4c253-139">String</span><span class="sxs-lookup"><span data-stu-id="4c253-139">String</span></span>|<span data-ttu-id="4c253-140">プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="4c253-140">The display name for the profile.</span></span>|
|<span data-ttu-id="4c253-141">会社</span><span class="sxs-lookup"><span data-stu-id="4c253-141">issuer</span></span>|[<span data-ttu-id="4c253-142">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="4c253-142">deviceManagementDerivedCredentialIssuer</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialissuer.md)|<span data-ttu-id="4c253-143">使用する派生資格情報プロバイダー。</span><span class="sxs-lookup"><span data-stu-id="4c253-143">The derived credential provider to use.</span></span> <span data-ttu-id="4c253-144">可能な値は、`intercede`、`entrustDatacard`、`purebred` です。</span><span class="sxs-lookup"><span data-stu-id="4c253-144">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="4c253-145">notificationType</span><span class="sxs-lookup"><span data-stu-id="4c253-145">notificationType</span></span>|[<span data-ttu-id="4c253-146">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="4c253-146">deviceManagementDerivedCredentialNotificationType</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialnotificationtype.md)|<span data-ttu-id="4c253-147">デバイスに証明書を使用する、Wi-fi、VPN、または電子メールプロファイルを配信するために、会社のポータルを開くことをエンドユーザーに通知するために使用されるメソッド。</span><span class="sxs-lookup"><span data-stu-id="4c253-147">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="4c253-148">可能な値は、`none`、`companyPortal`、`email` です。</span><span class="sxs-lookup"><span data-stu-id="4c253-148">Possible values are: `none`, `companyPortal`, `email`.</span></span>|



## <a name="response"></a><span data-ttu-id="4c253-149">応答</span><span class="sxs-lookup"><span data-stu-id="4c253-149">Response</span></span>
<span data-ttu-id="4c253-150">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4c253-150">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c253-151">例</span><span class="sxs-lookup"><span data-stu-id="4c253-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c253-152">要求</span><span class="sxs-lookup"><span data-stu-id="4c253-152">Request</span></span>
<span data-ttu-id="4c253-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4c253-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
Content-type: application/json
Content-length: 241

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "helpUrl": "https://example.com/helpUrl/",
  "displayName": "Display Name value",
  "issuer": "entrustDatacard",
  "notificationType": "companyPortal"
}
```

### <a name="response"></a><span data-ttu-id="4c253-154">応答</span><span class="sxs-lookup"><span data-stu-id="4c253-154">Response</span></span>
<span data-ttu-id="4c253-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4c253-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 290

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "bc650741-0741-bc65-4107-65bc410765bc",
  "helpUrl": "https://example.com/helpUrl/",
  "displayName": "Display Name value",
  "issuer": "entrustDatacard",
  "notificationType": "companyPortal"
}
```






