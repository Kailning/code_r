# **backend**

*   linux

    *   console

        *   spawnTerminalEmulator

*   mi2

    *   mi2.ts

        *   method

            *   escape

            *   couldBeOutput

        *   class MI2

            *   constructor

            *   getOriginallyNoTokenMINodes

            *   调试器控制

                *

                    *   load/attach/connect

                    *   ssh

                    *   initCommands

                *

                    *   start/stop/detach/interrupt/continue/next

                    *   step/stepInstructor/stepOut

                    *   goto

                    *   changeVariable

            *   数据/消息处理

                *   stdout/stderr

                *   onOutput/onOutPartial/onOutputStderr

            *   断点控制

                *   setEntryBreakPoint

                *   setBreakPointsCondition

                *   loadBreakPoints/addBreakPoints

                *   removeBreakPoints/clearBreakPoints

            *   文件

                *   addSymbleFile

                *   removeSymbleFile

            *   与调试器交互

                *

                    *   getThread

                    *   getStack/getStackVaribles

                    *   getRegisterNames/getRegistersNames

                    *   getRegisters/getSomeRegisters

                    *   getSmoeRegisterValues/getRegisterValues

            *   表达式/变量

                *   evalExpression/varEvalExpression

                *   varCreate/varUpdate/varAssign

                *   varListChidren

            *   发送命令

                *

                    *   sendRaw/sendUserInput

                    *   sendCommand/sendCliCommand

            *   examineMemory

            *   log/logNoNewLine

            *   isReady

            *   quote

    *   mi2lldb.ts

        *   initCommonds

        *   attach

        *   goto

        *   setBreakPointCndition

    *   mi2mago.ts

        *   getStack

*   backend.ts

    *   &#x20;ValuesFormattingMode

    *   interface

        *   Breakpoint/Thread/Stack/Variable/RegisterValue/SSHArguments/Register

        *   IBackend

            *   load/ssh/attach/connect/start/stop/detach/interrupt/continue/next/step/stepOut

            *   loadBreakPoints

            *   &#x9;addBreakPoint

            *   &#x9;removeBreakPoint

            *   &#x9;clearBreakPoints

            *   getThreads

            *   &#x9;getStack&#x20;

            *   &#x9;getStackVariables

            *   evalExpression

            *   &#x9;isReady

            *   &#x9;changeVariable

            *   &#x9;examineMemory

        *   MIError

            *   name/message /source

        *   MIErrorConstructor

            *   new

            *   prototype

    *   class

        *   VariableObject

            *   constructor

            *   applyChanges

            *   isCompound

            *   toProtocolVariable

        *   MIError

            *   \_message

            *   &#x20;\_source

            *   constructor

            *   &#x9;get message

            *   &#x9;get source

            *   get name

            *   &#x9;public toString

*   gdb\_expansion.ts

    *   isExpandable

    *   expandValue

        *   getNamespace

        *   parseCstring/ParseTurpleOrList/parsePrimitive

        *   createValue

        *   parseValue/parseCommonValue

        *   parseResult/parseCommonResult

*   mi\_parse.ts

    *   interface MIInfo

        *   token

        *   outOfBandRecord

            *   isStream

            *   type

            *   aysncClass

            *   outPut

            *   content

        *   resultRecords

    *   class MINode

        *   constructor

        *   record

        *   result

        *   valueOf

    *   function

        *   parseString

        *   ParseMI

            *   parseCString

            *   parseTupleOrList
