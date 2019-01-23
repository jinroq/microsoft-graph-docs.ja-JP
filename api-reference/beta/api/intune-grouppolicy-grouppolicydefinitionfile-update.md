---
title: GroupPolicyDefinitionFile を更新します。
description: GroupPolicyDefinitionFile オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be713dba2d503f19cd565fe5e53d252ed20667e0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430467"
---
# <a name="update-grouppolicydefinitionfile"></a><span data-ttu-id="7cf61-103">GroupPolicyDefinitionFile を更新します。</span><span class="sxs-lookup"><span data-stu-id="7cf61-103">Update groupPolicyDefinitionFile</span></span>

> <span data-ttu-id="7cf61-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7cf61-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7cf61-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cf61-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7cf61-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7cf61-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cf61-107">[GroupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7cf61-107">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7cf61-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7cf61-108">Prerequisites</span></span>
<span data-ttu-id="7cf61-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7cf61-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7cf61-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7cf61-111">Permission type</span></span>|<span data-ttu-id="7cf61-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7cf61-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cf61-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7cf61-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7cf61-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cf61-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7cf61-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7cf61-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cf61-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cf61-116">Not supported.</span></span>|
|<span data-ttu-id="7cf61-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7cf61-117">Application</span></span>|<span data-ttu-id="7cf61-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cf61-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cf61-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7cf61-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
```

## <a name="request-headers"></a><span data-ttu-id="7cf61-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7cf61-120">Request headers</span></span>
|<span data-ttu-id="7cf61-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7cf61-121">Header</span></span>|<span data-ttu-id="7cf61-122">値</span><span class="sxs-lookup"><span data-stu-id="7cf61-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cf61-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cf61-123">Authorization</span></span>|<span data-ttu-id="7cf61-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7cf61-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cf61-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7cf61-125">Accept</span></span>|<span data-ttu-id="7cf61-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7cf61-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cf61-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7cf61-127">Request body</span></span>
<span data-ttu-id="7cf61-128">要求の本文に[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="7cf61-128">In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

<span data-ttu-id="7cf61-129">[GroupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="7cf61-129">The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span>

|<span data-ttu-id="7cf61-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7cf61-130">Property</span></span>|<span data-ttu-id="7cf61-131">型</span><span class="sxs-lookup"><span data-stu-id="7cf61-131">Type</span></span>|<span data-ttu-id="7cf61-132">説明</span><span class="sxs-lookup"><span data-stu-id="7cf61-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cf61-133">displayName</span><span class="sxs-lookup"><span data-stu-id="7cf61-133">displayName</span></span>|<span data-ttu-id="7cf61-134">String</span><span class="sxs-lookup"><span data-stu-id="7cf61-134">String</span></span>|<span data-ttu-id="7cf61-135">ADMX ファイルのローカライズされた表示名です。</span><span class="sxs-lookup"><span data-stu-id="7cf61-135">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="7cf61-136">説明</span><span class="sxs-lookup"><span data-stu-id="7cf61-136">description</span></span>|<span data-ttu-id="7cf61-137">String</span><span class="sxs-lookup"><span data-stu-id="7cf61-137">String</span></span>|<span data-ttu-id="7cf61-138">ADMX ファイル内のポリシー設定のローカライズされた説明。</span><span class="sxs-lookup"><span data-stu-id="7cf61-138">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="7cf61-139">既定値は空です。</span><span class="sxs-lookup"><span data-stu-id="7cf61-139">The default value is empty.</span></span>|
|<span data-ttu-id="7cf61-140">languageCodes</span><span class="sxs-lookup"><span data-stu-id="7cf61-140">languageCodes</span></span>|<span data-ttu-id="7cf61-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7cf61-141">String collection</span></span>|<span data-ttu-id="7cf61-142">ADMX ファイルのサポートされている言語コードです。</span><span class="sxs-lookup"><span data-stu-id="7cf61-142">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="7cf61-143">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="7cf61-143">targetPrefix</span></span>|<span data-ttu-id="7cf61-144">String</span><span class="sxs-lookup"><span data-stu-id="7cf61-144">String</span></span>|<span data-ttu-id="7cf61-145">ADMX ファイル内で名前空間を参照する論理名を指定します。</span><span class="sxs-lookup"><span data-stu-id="7cf61-145">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="7cf61-146">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="7cf61-146">targetNamespace</span></span>|<span data-ttu-id="7cf61-147">String</span><span class="sxs-lookup"><span data-stu-id="7cf61-147">String</span></span>|<span data-ttu-id="7cf61-148">ADMX ファイル内で名前空間を識別するために使用する URI を指定します。</span><span class="sxs-lookup"><span data-stu-id="7cf61-148">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="7cf61-149">policyType</span><span class="sxs-lookup"><span data-stu-id="7cf61-149">policyType</span></span>|[<span data-ttu-id="7cf61-150">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="7cf61-150">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="7cf61-151">グループ ポリシーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="7cf61-151">Specifies the type of group policy.</span></span> <span data-ttu-id="7cf61-152">使用可能な値は、`admxBacked`、`admxIngested` です。</span><span class="sxs-lookup"><span data-stu-id="7cf61-152">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="7cf61-153">id</span><span class="sxs-lookup"><span data-stu-id="7cf61-153">id</span></span>|<span data-ttu-id="7cf61-154">String</span><span class="sxs-lookup"><span data-stu-id="7cf61-154">String</span></span>|<span data-ttu-id="7cf61-155">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7cf61-155">Key of the entity.</span></span>|
|<span data-ttu-id="7cf61-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7cf61-156">lastModifiedDateTime</span></span>|<span data-ttu-id="7cf61-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cf61-157">DateTimeOffset</span></span>|<span data-ttu-id="7cf61-158">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="7cf61-158">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="7cf61-159">応答</span><span class="sxs-lookup"><span data-stu-id="7cf61-159">Response</span></span>
<span data-ttu-id="7cf61-160">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7cf61-160">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cf61-161">例</span><span class="sxs-lookup"><span data-stu-id="7cf61-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="7cf61-162">要求</span><span class="sxs-lookup"><span data-stu-id="7cf61-162">Request</span></span>
<span data-ttu-id="7cf61-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7cf61-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7cf61-164">応答</span><span class="sxs-lookup"><span data-stu-id="7cf61-164">Response</span></span>
<span data-ttu-id="7cf61-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7cf61-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




