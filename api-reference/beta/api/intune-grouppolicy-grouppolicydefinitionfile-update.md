---
title: grouppolicydefinitionfile の更新
description: grouppolicydefinitionfile オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e204382f9237428b30362f7464264f732e13541a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169413"
---
# <a name="update-grouppolicydefinitionfile"></a><span data-ttu-id="8c506-103">grouppolicydefinitionfile の更新</span><span class="sxs-lookup"><span data-stu-id="8c506-103">Update groupPolicyDefinitionFile</span></span>

> <span data-ttu-id="8c506-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c506-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c506-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8c506-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c506-106">[grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8c506-106">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c506-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8c506-107">Prerequisites</span></span>
<span data-ttu-id="8c506-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c506-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8c506-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8c506-110">Permission type</span></span>|<span data-ttu-id="8c506-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8c506-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c506-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8c506-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8c506-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c506-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8c506-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8c506-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c506-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c506-115">Not supported.</span></span>|
|<span data-ttu-id="8c506-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8c506-116">Application</span></span>|<span data-ttu-id="8c506-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c506-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c506-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8c506-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
```

## <a name="request-headers"></a><span data-ttu-id="8c506-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c506-119">Request headers</span></span>
|<span data-ttu-id="8c506-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c506-120">Header</span></span>|<span data-ttu-id="8c506-121">値</span><span class="sxs-lookup"><span data-stu-id="8c506-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c506-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c506-122">Authorization</span></span>|<span data-ttu-id="8c506-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8c506-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c506-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8c506-124">Accept</span></span>|<span data-ttu-id="8c506-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8c506-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c506-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8c506-126">Request body</span></span>
<span data-ttu-id="8c506-127">要求本文で、 [grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8c506-127">In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

<span data-ttu-id="8c506-128">次の表に、 [grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8c506-128">The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span>

|<span data-ttu-id="8c506-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c506-129">Property</span></span>|<span data-ttu-id="8c506-130">型</span><span class="sxs-lookup"><span data-stu-id="8c506-130">Type</span></span>|<span data-ttu-id="8c506-131">説明</span><span class="sxs-lookup"><span data-stu-id="8c506-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c506-132">displayName</span><span class="sxs-lookup"><span data-stu-id="8c506-132">displayName</span></span>|<span data-ttu-id="8c506-133">String</span><span class="sxs-lookup"><span data-stu-id="8c506-133">String</span></span>|<span data-ttu-id="8c506-134">ADMX ファイルのローカライズされたフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="8c506-134">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="8c506-135">説明</span><span class="sxs-lookup"><span data-stu-id="8c506-135">description</span></span>|<span data-ttu-id="8c506-136">String</span><span class="sxs-lookup"><span data-stu-id="8c506-136">String</span></span>|<span data-ttu-id="8c506-137">ADMX ファイルのポリシー設定のローカライズされた説明。</span><span class="sxs-lookup"><span data-stu-id="8c506-137">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="8c506-138">既定値は empty です。</span><span class="sxs-lookup"><span data-stu-id="8c506-138">The default value is empty.</span></span>|
|<span data-ttu-id="8c506-139">languageCodes</span><span class="sxs-lookup"><span data-stu-id="8c506-139">languageCodes</span></span>|<span data-ttu-id="8c506-140">String collection</span><span class="sxs-lookup"><span data-stu-id="8c506-140">String collection</span></span>|<span data-ttu-id="8c506-141">ADMX ファイルでサポートされている言語コード。</span><span class="sxs-lookup"><span data-stu-id="8c506-141">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="8c506-142">targetprefix</span><span class="sxs-lookup"><span data-stu-id="8c506-142">targetPrefix</span></span>|<span data-ttu-id="8c506-143">String</span><span class="sxs-lookup"><span data-stu-id="8c506-143">String</span></span>|<span data-ttu-id="8c506-144">ADMX ファイル内の名前空間を参照する論理名を指定します。</span><span class="sxs-lookup"><span data-stu-id="8c506-144">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="8c506-145">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="8c506-145">targetNamespace</span></span>|<span data-ttu-id="8c506-146">String</span><span class="sxs-lookup"><span data-stu-id="8c506-146">String</span></span>|<span data-ttu-id="8c506-147">ADMX ファイル内の名前空間を識別するために使用する URI を指定します。</span><span class="sxs-lookup"><span data-stu-id="8c506-147">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="8c506-148">msrtcsip-policytype</span><span class="sxs-lookup"><span data-stu-id="8c506-148">policyType</span></span>|[<span data-ttu-id="8c506-149">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="8c506-149">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="8c506-150">グループポリシーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="8c506-150">Specifies the type of group policy.</span></span> <span data-ttu-id="8c506-151">使用可能な値は、`admxBacked`、`admxIngested` です。</span><span class="sxs-lookup"><span data-stu-id="8c506-151">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="8c506-152">id</span><span class="sxs-lookup"><span data-stu-id="8c506-152">id</span></span>|<span data-ttu-id="8c506-153">String</span><span class="sxs-lookup"><span data-stu-id="8c506-153">String</span></span>|<span data-ttu-id="8c506-154">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8c506-154">Key of the entity.</span></span>|
|<span data-ttu-id="8c506-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c506-155">lastModifiedDateTime</span></span>|<span data-ttu-id="8c506-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c506-156">DateTimeOffset</span></span>|<span data-ttu-id="8c506-157">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="8c506-157">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="8c506-158">応答</span><span class="sxs-lookup"><span data-stu-id="8c506-158">Response</span></span>
<span data-ttu-id="8c506-159">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8c506-159">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c506-160">例</span><span class="sxs-lookup"><span data-stu-id="8c506-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c506-161">要求</span><span class="sxs-lookup"><span data-stu-id="8c506-161">Request</span></span>
<span data-ttu-id="8c506-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8c506-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested"
}
```

### <a name="response"></a><span data-ttu-id="8c506-163">応答</span><span class="sxs-lookup"><span data-stu-id="8c506-163">Response</span></span>
<span data-ttu-id="8c506-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8c506-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 438

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "id": "940aa2a1-a2a1-940a-a1a2-0a94a1a20a94",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




