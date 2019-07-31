---
title: registryKeyState リソースの種類
description: 通知に関連するレジストリキーの変更に関する情報、およびレジストリキーを変更したプロセスについて説明します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 672a782b97b3a96c9a7065f3bf5c7b5b9030f282
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965454"
---
# <a name="registrykeystate-resource-type"></a><span data-ttu-id="be84d-103">registryKeyState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="be84d-103">registryKeyState resource type</span></span>

<span data-ttu-id="be84d-104">通知に関連するレジストリキーの変更に関する情報、およびレジストリキーを変更したプロセスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="be84d-104">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="be84d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be84d-105">Properties</span></span>

| <span data-ttu-id="be84d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be84d-106">Property</span></span>     | <span data-ttu-id="be84d-107">型</span><span class="sxs-lookup"><span data-stu-id="be84d-107">Type</span></span>        | <span data-ttu-id="be84d-108">説明</span><span class="sxs-lookup"><span data-stu-id="be84d-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="be84d-109">レジストリ</span><span class="sxs-lookup"><span data-stu-id="be84d-109">hive</span></span>|<span data-ttu-id="be84d-110">registryHive</span><span class="sxs-lookup"><span data-stu-id="be84d-110">registryHive</span></span>|<span data-ttu-id="be84d-111">[Windows レジストリハイブ](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives):</span><span class="sxs-lookup"><span data-stu-id="be84d-111">A [Windows registry hive](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="be84d-112">HKEY_CURRENT_CONFIG</span><span class="sxs-lookup"><span data-stu-id="be84d-112">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="be84d-113">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="be84d-113">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="be84d-114">HKEY_LOCAL_MACHINE\SAM</span><span class="sxs-lookup"><span data-stu-id="be84d-114">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="be84d-115">HKEY_LOCAL_MACHINE\Security</span><span class="sxs-lookup"><span data-stu-id="be84d-115">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="be84d-116">HKEY_LOCAL_MACHINE\Software</span><span class="sxs-lookup"><span data-stu-id="be84d-116">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="be84d-117">HKEY_LOCAL_MACHINE\System</span><span class="sxs-lookup"><span data-stu-id="be84d-117">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="be84d-118">HKEY_USERS\\限り.</span><span class="sxs-lookup"><span data-stu-id="be84d-118">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="be84d-119">可能な値は、`unknown`、`currentConfig`、`currentUser`、`localMachineSam`、`localMachineSecurity`、`localMachineSoftware`、`localMachineSystem`、`usersDefault` です。</span><span class="sxs-lookup"><span data-stu-id="be84d-119">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="be84d-120">キー</span><span class="sxs-lookup"><span data-stu-id="be84d-120">key</span></span>|<span data-ttu-id="be84d-121">String</span><span class="sxs-lookup"><span data-stu-id="be84d-121">String</span></span>|<span data-ttu-id="be84d-122">Current (つまり変更された) レジストリキー (ハイブを除外)。</span><span class="sxs-lookup"><span data-stu-id="be84d-122">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="be84d-123">oldKey</span><span class="sxs-lookup"><span data-stu-id="be84d-123">oldKey</span></span>|<span data-ttu-id="be84d-124">String</span><span class="sxs-lookup"><span data-stu-id="be84d-124">String</span></span>|<span data-ttu-id="be84d-125">Previous (変更前) レジストリキー (ハイブを除外)。</span><span class="sxs-lookup"><span data-stu-id="be84d-125">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="be84d-126">oldValueData</span><span class="sxs-lookup"><span data-stu-id="be84d-126">oldValueData</span></span>|<span data-ttu-id="be84d-127">String</span><span class="sxs-lookup"><span data-stu-id="be84d-127">String</span></span>|<span data-ttu-id="be84d-128">以前の (変更前) レジストリキー値のデータ (内容)。</span><span class="sxs-lookup"><span data-stu-id="be84d-128">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="be84d-129">oldValueName</span><span class="sxs-lookup"><span data-stu-id="be84d-129">oldValueName</span></span>|<span data-ttu-id="be84d-130">String</span><span class="sxs-lookup"><span data-stu-id="be84d-130">String</span></span>|<span data-ttu-id="be84d-131">Previous (変更前) レジストリキー値の名前。</span><span class="sxs-lookup"><span data-stu-id="be84d-131">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="be84d-132">operation</span><span class="sxs-lookup"><span data-stu-id="be84d-132">operation</span></span>|<span data-ttu-id="be84d-133">registryOperation</span><span class="sxs-lookup"><span data-stu-id="be84d-133">registryOperation</span></span>|<span data-ttu-id="be84d-134">レジストリキー名と値の一方または両方を変更した操作。</span><span class="sxs-lookup"><span data-stu-id="be84d-134">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="be84d-135">使用可能な値は、`unknown`、`create`、`modify`、`delete` です。</span><span class="sxs-lookup"><span data-stu-id="be84d-135">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="be84d-136">processId</span><span class="sxs-lookup"><span data-stu-id="be84d-136">processId</span></span>|<span data-ttu-id="be84d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="be84d-137">Int32</span></span>|<span data-ttu-id="be84d-138">レジストリキーを変更したプロセスのプロセス ID (PID) (プロセスの詳細は、警告の「プロセス」のコレクションに表示されます)。</span><span class="sxs-lookup"><span data-stu-id="be84d-138">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="be84d-139">valueData</span><span class="sxs-lookup"><span data-stu-id="be84d-139">valueData</span></span>|<span data-ttu-id="be84d-140">String</span><span class="sxs-lookup"><span data-stu-id="be84d-140">String</span></span>|<span data-ttu-id="be84d-141">現在の (つまり変更された) レジストリキー値のデータ (内容)。</span><span class="sxs-lookup"><span data-stu-id="be84d-141">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="be84d-142">valueName</span><span class="sxs-lookup"><span data-stu-id="be84d-142">valueName</span></span>|<span data-ttu-id="be84d-143">String</span><span class="sxs-lookup"><span data-stu-id="be84d-143">String</span></span>|<span data-ttu-id="be84d-144">Current (変更された) レジストリキー値の名前</span><span class="sxs-lookup"><span data-stu-id="be84d-144">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="be84d-145">valueType</span><span class="sxs-lookup"><span data-stu-id="be84d-145">valueType</span></span>|<span data-ttu-id="be84d-146">registryValueType</span><span class="sxs-lookup"><span data-stu-id="be84d-146">registryValueType</span></span>|[<span data-ttu-id="be84d-147">レジストリキーの値の種類</span><span class="sxs-lookup"><span data-stu-id="be84d-147">Registry key value type</span></span>](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="be84d-148">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="be84d-148">REG_BINARY</span></span></li> <li><span data-ttu-id="be84d-149">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="be84d-149">REG_DWORD</span></span></li> <li><span data-ttu-id="be84d-150">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="be84d-150">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="be84d-151">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="be84d-151">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="be84d-152">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="be84d-152">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="be84d-153">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="be84d-153">REG_LINK</span></span></li> <li><span data-ttu-id="be84d-154">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="be84d-154">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="be84d-155">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="be84d-155">REG_NONE</span></span></li> <li><span data-ttu-id="be84d-156">REG_QWORD</span><span class="sxs-lookup"><span data-stu-id="be84d-156">REG_QWORD</span></span></li> <li><span data-ttu-id="be84d-157">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="be84d-157">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="be84d-158">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="be84d-158">REG_SZ</span></span></li></ul> <span data-ttu-id="be84d-159">可能な値は、`unknown`、`binary`、`dword`、`dwordLittleEndian`、`dwordBigEndian`、`expandSz`、`link`、`multiSz`、`none`、`qword`、`qwordlittleEndian`、`sz` です。</span><span class="sxs-lookup"><span data-stu-id="be84d-159">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be84d-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="be84d-160">JSON representation</span></span>

<span data-ttu-id="be84d-161">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="be84d-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.registryKeyState"
}-->

```json
{
  "hive": "@odata.type: microsoft.graph.registryHive",
  "key": "String",
  "oldKey": "String",
  "oldValueData": "String",
  "oldValueName": "String",
  "operation": "@odata.type: microsoft.graph.registryOperation",
  "processId": 1024,
  "valueData": "String",
  "valueName": "String",
  "valueType": "@odata.type: microsoft.graph.registryValueType"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "registryKeyState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
