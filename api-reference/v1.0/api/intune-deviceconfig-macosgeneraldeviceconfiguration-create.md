---
title: Create macOSGeneralDeviceConfiguration
description: 新しい macOSGeneralDeviceConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e69f60508ae7e82c071024f0a703141c78200a1c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017127"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="84e9a-103">Create macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="84e9a-103">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="84e9a-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="84e9a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84e9a-105">新しい [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="84e9a-105">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84e9a-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="84e9a-106">Prerequisites</span></span>
<span data-ttu-id="84e9a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84e9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84e9a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="84e9a-109">Permission type</span></span>|<span data-ttu-id="84e9a-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="84e9a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84e9a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="84e9a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="84e9a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84e9a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84e9a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="84e9a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84e9a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84e9a-114">Not supported.</span></span>|
|<span data-ttu-id="84e9a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="84e9a-115">Application</span></span>|<span data-ttu-id="84e9a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84e9a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84e9a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="84e9a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="84e9a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="84e9a-118">Request headers</span></span>
|<span data-ttu-id="84e9a-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="84e9a-119">Header</span></span>|<span data-ttu-id="84e9a-120">値</span><span class="sxs-lookup"><span data-stu-id="84e9a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84e9a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="84e9a-121">Authorization</span></span>|<span data-ttu-id="84e9a-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="84e9a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84e9a-123">承諾</span><span class="sxs-lookup"><span data-stu-id="84e9a-123">Accept</span></span>|<span data-ttu-id="84e9a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="84e9a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84e9a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="84e9a-125">Request body</span></span>
<span data-ttu-id="84e9a-126">要求本文で、macOSGeneralDeviceConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="84e9a-126">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="84e9a-127">次の表に、macOSGeneralDeviceConfiguration 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="84e9a-127">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="84e9a-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84e9a-128">Property</span></span>|<span data-ttu-id="84e9a-129">型</span><span class="sxs-lookup"><span data-stu-id="84e9a-129">Type</span></span>|<span data-ttu-id="84e9a-130">説明</span><span class="sxs-lookup"><span data-stu-id="84e9a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84e9a-131">id</span><span class="sxs-lookup"><span data-stu-id="84e9a-131">id</span></span>|<span data-ttu-id="84e9a-132">文字列</span><span class="sxs-lookup"><span data-stu-id="84e9a-132">String</span></span>|<span data-ttu-id="84e9a-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="84e9a-133">Key of the entity.</span></span> <span data-ttu-id="84e9a-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="84e9a-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84e9a-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84e9a-135">lastModifiedDateTime</span></span>|<span data-ttu-id="84e9a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84e9a-136">DateTimeOffset</span></span>|<span data-ttu-id="84e9a-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="84e9a-137">DateTime the object was last modified.</span></span> <span data-ttu-id="84e9a-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="84e9a-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84e9a-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84e9a-139">createdDateTime</span></span>|<span data-ttu-id="84e9a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84e9a-140">DateTimeOffset</span></span>|<span data-ttu-id="84e9a-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="84e9a-141">DateTime the object was created.</span></span> <span data-ttu-id="84e9a-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="84e9a-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84e9a-143">description</span><span class="sxs-lookup"><span data-stu-id="84e9a-143">description</span></span>|<span data-ttu-id="84e9a-144">String</span><span class="sxs-lookup"><span data-stu-id="84e9a-144">String</span></span>|<span data-ttu-id="84e9a-145">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="84e9a-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="84e9a-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="84e9a-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84e9a-147">displayName</span><span class="sxs-lookup"><span data-stu-id="84e9a-147">displayName</span></span>|<span data-ttu-id="84e9a-148">String</span><span class="sxs-lookup"><span data-stu-id="84e9a-148">String</span></span>|<span data-ttu-id="84e9a-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="84e9a-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="84e9a-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="84e9a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84e9a-151">version</span><span class="sxs-lookup"><span data-stu-id="84e9a-151">version</span></span>|<span data-ttu-id="84e9a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="84e9a-152">Int32</span></span>|<span data-ttu-id="84e9a-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="84e9a-153">Version of the device configuration.</span></span> <span data-ttu-id="84e9a-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="84e9a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84e9a-155">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="84e9a-155">compliantAppsList</span></span>|<span data-ttu-id="84e9a-156">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="84e9a-156">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="84e9a-157">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="84e9a-157">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="84e9a-158">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="84e9a-158">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="84e9a-159">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="84e9a-159">compliantAppListType</span></span>|[<span data-ttu-id="84e9a-160">アプライアンスの種類</span><span class="sxs-lookup"><span data-stu-id="84e9a-160">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="84e9a-161">CompliantAppsList 内にあるリスト。</span><span class="sxs-lookup"><span data-stu-id="84e9a-161">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="84e9a-162">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="84e9a-162">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="84e9a-163">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="84e9a-163">emailInDomainSuffixes</span></span>|<span data-ttu-id="84e9a-164">String コレクション</span><span class="sxs-lookup"><span data-stu-id="84e9a-164">String collection</span></span>|<span data-ttu-id="84e9a-165">これらの文字列のいずれかに一致するサフィックスがないメール アドレスは、ドメイン外と見なされます。</span><span class="sxs-lookup"><span data-stu-id="84e9a-165">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="84e9a-166">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="84e9a-166">passwordBlockSimple</span></span>|<span data-ttu-id="84e9a-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="84e9a-167">Boolean</span></span>|<span data-ttu-id="84e9a-168">単純なパスワードを禁止します。</span><span class="sxs-lookup"><span data-stu-id="84e9a-168">Block simple passwords.</span></span>|
|<span data-ttu-id="84e9a-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="84e9a-169">passwordExpirationDays</span></span>|<span data-ttu-id="84e9a-170">Int32</span><span class="sxs-lookup"><span data-stu-id="84e9a-170">Int32</span></span>|<span data-ttu-id="84e9a-171">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="84e9a-171">Number of days before the password expires.</span></span>|
|<span data-ttu-id="84e9a-172">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="84e9a-172">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="84e9a-173">Int32</span><span class="sxs-lookup"><span data-stu-id="84e9a-173">Int32</span></span>|<span data-ttu-id="84e9a-174">パスワードが含まなければならない文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="84e9a-174">Number of character sets a password must contain.</span></span> <span data-ttu-id="84e9a-175">有効な値は 0 から 4 までです</span><span class="sxs-lookup"><span data-stu-id="84e9a-175">Valid values 0 to 4</span></span>|
|<span data-ttu-id="84e9a-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="84e9a-176">passwordMinimumLength</span></span>|<span data-ttu-id="84e9a-177">Int32</span><span class="sxs-lookup"><span data-stu-id="84e9a-177">Int32</span></span>|<span data-ttu-id="84e9a-178">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="84e9a-178">Minimum length of passwords.</span></span>|
|<span data-ttu-id="84e9a-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="84e9a-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="84e9a-180">Int32</span><span class="sxs-lookup"><span data-stu-id="84e9a-180">Int32</span></span>|<span data-ttu-id="84e9a-181">パスワードが要求されるまでに必要な非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="84e9a-181">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="84e9a-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="84e9a-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="84e9a-183">Int32</span><span class="sxs-lookup"><span data-stu-id="84e9a-183">Int32</span></span>|<span data-ttu-id="84e9a-184">画面がタイムアウトになるまでに必要な非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="84e9a-184">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="84e9a-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="84e9a-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="84e9a-186">Int32</span><span class="sxs-lookup"><span data-stu-id="84e9a-186">Int32</span></span>|<span data-ttu-id="84e9a-187">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="84e9a-187">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="84e9a-188">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="84e9a-188">passwordRequiredType</span></span>|[<span data-ttu-id="84e9a-189">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="84e9a-189">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="84e9a-190">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="84e9a-190">Type of password that is required.</span></span> <span data-ttu-id="84e9a-191">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="84e9a-191">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="84e9a-192">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="84e9a-192">passwordRequired</span></span>|<span data-ttu-id="84e9a-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="84e9a-193">Boolean</span></span>|<span data-ttu-id="84e9a-194">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="84e9a-194">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="84e9a-195">応答</span><span class="sxs-lookup"><span data-stu-id="84e9a-195">Response</span></span>
<span data-ttu-id="84e9a-196">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="84e9a-196">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84e9a-197">例</span><span class="sxs-lookup"><span data-stu-id="84e9a-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="84e9a-198">要求</span><span class="sxs-lookup"><span data-stu-id="84e9a-198">Request</span></span>
<span data-ttu-id="84e9a-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="84e9a-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 906

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true
}
```

### <a name="response"></a><span data-ttu-id="84e9a-200">応答</span><span class="sxs-lookup"><span data-stu-id="84e9a-200">Response</span></span>
<span data-ttu-id="84e9a-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="84e9a-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1078

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true
}
```



