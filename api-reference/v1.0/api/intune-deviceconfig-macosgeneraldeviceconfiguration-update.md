---
title: macOSGeneralDeviceConfiguration の更新
description: macOSGeneralDeviceConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 70a1147fe3b3f2731dc6fa7a884931e04dd3bcee
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914820"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="cdaef-103">macOSGeneralDeviceConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="cdaef-103">Update macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="cdaef-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cdaef-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cdaef-105">[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cdaef-105">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cdaef-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="cdaef-106">Prerequisites</span></span>
<span data-ttu-id="cdaef-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cdaef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdaef-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cdaef-109">Permission type</span></span>|<span data-ttu-id="cdaef-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cdaef-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdaef-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cdaef-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cdaef-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdaef-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cdaef-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cdaef-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdaef-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cdaef-114">Not supported.</span></span>|
|<span data-ttu-id="cdaef-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cdaef-115">Application</span></span>|<span data-ttu-id="cdaef-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cdaef-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdaef-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cdaef-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cdaef-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cdaef-118">Request headers</span></span>
|<span data-ttu-id="cdaef-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cdaef-119">Header</span></span>|<span data-ttu-id="cdaef-120">値</span><span class="sxs-lookup"><span data-stu-id="cdaef-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdaef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdaef-121">Authorization</span></span>|<span data-ttu-id="cdaef-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cdaef-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdaef-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cdaef-123">Accept</span></span>|<span data-ttu-id="cdaef-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cdaef-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdaef-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="cdaef-125">Request body</span></span>
<span data-ttu-id="cdaef-126">要求本文で、[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cdaef-126">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="cdaef-127">次の表に、[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cdaef-127">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="cdaef-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cdaef-128">Property</span></span>|<span data-ttu-id="cdaef-129">型</span><span class="sxs-lookup"><span data-stu-id="cdaef-129">Type</span></span>|<span data-ttu-id="cdaef-130">説明</span><span class="sxs-lookup"><span data-stu-id="cdaef-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdaef-131">ID</span><span class="sxs-lookup"><span data-stu-id="cdaef-131">id</span></span>|<span data-ttu-id="cdaef-132">String</span><span class="sxs-lookup"><span data-stu-id="cdaef-132">String</span></span>|<span data-ttu-id="cdaef-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cdaef-133">Key of the entity.</span></span> <span data-ttu-id="cdaef-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cdaef-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cdaef-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cdaef-135">lastModifiedDateTime</span></span>|<span data-ttu-id="cdaef-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdaef-136">DateTimeOffset</span></span>|<span data-ttu-id="cdaef-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="cdaef-137">DateTime the object was last modified.</span></span> <span data-ttu-id="cdaef-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cdaef-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cdaef-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cdaef-139">createdDateTime</span></span>|<span data-ttu-id="cdaef-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cdaef-140">DateTimeOffset</span></span>|<span data-ttu-id="cdaef-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="cdaef-141">DateTime the object was created.</span></span> <span data-ttu-id="cdaef-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cdaef-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cdaef-143">説明</span><span class="sxs-lookup"><span data-stu-id="cdaef-143">description</span></span>|<span data-ttu-id="cdaef-144">String</span><span class="sxs-lookup"><span data-stu-id="cdaef-144">String</span></span>|<span data-ttu-id="cdaef-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="cdaef-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cdaef-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cdaef-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cdaef-147">displayName</span><span class="sxs-lookup"><span data-stu-id="cdaef-147">displayName</span></span>|<span data-ttu-id="cdaef-148">String</span><span class="sxs-lookup"><span data-stu-id="cdaef-148">String</span></span>|<span data-ttu-id="cdaef-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="cdaef-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cdaef-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cdaef-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cdaef-151">version</span><span class="sxs-lookup"><span data-stu-id="cdaef-151">version</span></span>|<span data-ttu-id="cdaef-152">Int32</span><span class="sxs-lookup"><span data-stu-id="cdaef-152">Int32</span></span>|<span data-ttu-id="cdaef-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="cdaef-153">Version of the device configuration.</span></span> <span data-ttu-id="cdaef-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="cdaef-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cdaef-155">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="cdaef-155">compliantAppsList</span></span>|<span data-ttu-id="cdaef-156">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cdaef-156">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="cdaef-157">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="cdaef-157">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="cdaef-158">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="cdaef-158">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="cdaef-159">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="cdaef-159">compliantAppListType</span></span>|[<span data-ttu-id="cdaef-160">appListType</span><span class="sxs-lookup"><span data-stu-id="cdaef-160">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="cdaef-161">CompliantAppsList 内にあるリスト。</span><span class="sxs-lookup"><span data-stu-id="cdaef-161">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="cdaef-162">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="cdaef-162">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="cdaef-163">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="cdaef-163">emailInDomainSuffixes</span></span>|<span data-ttu-id="cdaef-164">String コレクション</span><span class="sxs-lookup"><span data-stu-id="cdaef-164">String collection</span></span>|<span data-ttu-id="cdaef-165">これらの文字列のいずれかに一致するサフィックスがないメール アドレスは、ドメイン外と見なされます。</span><span class="sxs-lookup"><span data-stu-id="cdaef-165">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="cdaef-166">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="cdaef-166">passwordBlockSimple</span></span>|<span data-ttu-id="cdaef-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="cdaef-167">Boolean</span></span>|<span data-ttu-id="cdaef-168">単純なパスワードを禁止します。</span><span class="sxs-lookup"><span data-stu-id="cdaef-168">Block simple passwords.</span></span>|
|<span data-ttu-id="cdaef-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="cdaef-169">passwordExpirationDays</span></span>|<span data-ttu-id="cdaef-170">Int32</span><span class="sxs-lookup"><span data-stu-id="cdaef-170">Int32</span></span>|<span data-ttu-id="cdaef-171">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="cdaef-171">Number of days before the password expires.</span></span>|
|<span data-ttu-id="cdaef-172">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="cdaef-172">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="cdaef-173">Int32</span><span class="sxs-lookup"><span data-stu-id="cdaef-173">Int32</span></span>|<span data-ttu-id="cdaef-174">パスワードが含まなければならない文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="cdaef-174">Number of character sets a password must contain.</span></span> <span data-ttu-id="cdaef-175">有効な値は 0 から 4 までです</span><span class="sxs-lookup"><span data-stu-id="cdaef-175">Valid values 0 to 4</span></span>|
|<span data-ttu-id="cdaef-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="cdaef-176">passwordMinimumLength</span></span>|<span data-ttu-id="cdaef-177">Int32</span><span class="sxs-lookup"><span data-stu-id="cdaef-177">Int32</span></span>|<span data-ttu-id="cdaef-178">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="cdaef-178">Minimum length of passwords.</span></span>|
|<span data-ttu-id="cdaef-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="cdaef-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="cdaef-180">Int32</span><span class="sxs-lookup"><span data-stu-id="cdaef-180">Int32</span></span>|<span data-ttu-id="cdaef-181">パスワードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="cdaef-181">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="cdaef-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="cdaef-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="cdaef-183">Int32</span><span class="sxs-lookup"><span data-stu-id="cdaef-183">Int32</span></span>|<span data-ttu-id="cdaef-184">画面がタイムアウトになるまでの非アクティブ時間。</span><span class="sxs-lookup"><span data-stu-id="cdaef-184">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="cdaef-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="cdaef-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="cdaef-186">Int32</span><span class="sxs-lookup"><span data-stu-id="cdaef-186">Int32</span></span>|<span data-ttu-id="cdaef-187">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="cdaef-187">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="cdaef-188">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="cdaef-188">passwordRequiredType</span></span>|[<span data-ttu-id="cdaef-189">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="cdaef-189">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="cdaef-190">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="cdaef-190">Type of password that is required.</span></span> <span data-ttu-id="cdaef-191">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="cdaef-191">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="cdaef-192">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="cdaef-192">passwordRequired</span></span>|<span data-ttu-id="cdaef-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="cdaef-193">Boolean</span></span>|<span data-ttu-id="cdaef-194">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="cdaef-194">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="cdaef-195">応答</span><span class="sxs-lookup"><span data-stu-id="cdaef-195">Response</span></span>
<span data-ttu-id="cdaef-196">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="cdaef-196">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdaef-197">例</span><span class="sxs-lookup"><span data-stu-id="cdaef-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="cdaef-198">要求</span><span class="sxs-lookup"><span data-stu-id="cdaef-198">Request</span></span>
<span data-ttu-id="cdaef-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cdaef-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="cdaef-200">応答</span><span class="sxs-lookup"><span data-stu-id="cdaef-200">Response</span></span>
<span data-ttu-id="cdaef-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cdaef-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



